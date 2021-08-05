<script>
	export let menuMobile = false;
	export let menuDropdown = false;
	import {User} from '../../models/user';
	import UserMenu from './header/UserMenu.svelte';
	import { scrollto } from "svelte-scrollto";
	let user = User.getUser();
</script>
<svelte:head>
	{#if menuMobile}
		<style>
			body {
				overflow: hidden;
			}
		</style>
	{/if}
</svelte:head>
<header>
	<div class="row no-gutters">
		<button class="menu-btn" class:open="{menuMobile}" on:click={()=>{ menuMobile = !menuMobile; return false; }}>
			<svg width=32 height=24>
				<line id="top" x1=0 y1=2  x2=32 y2=2/>
				<line id="middle" x1=0 y1=12 x2=32 y2=12/>
				<line id="bottom" x1=0 y1=22 x2=32 y2=22/>
			</svg>
		</button>
		<!-- <div class="col-lg-2 col-sm-12 col-xs-11">
			<a href="/" class="brand-logo">
				<img src="/images/logo-conquest-small.png" alt="Logo">
			</a>
		</div> -->
		<div class="col-lg-12 col-sm-12 col-xs-12 menu-sec">
			<a href="/" class="brand-logo">
				<img src="/images/logo-conquest-small.png" alt="Logo">
			</a>
			<div class="menu-block" class:menuopen="{menuMobile}">
				<ul class="menu">
					<li>
						<a href="/">
							Home
						</a>
					</li>
					<!-- <li>
						<a href="/format">
							Format
						</a>
					</li>
					<li>
						<a href="/schedule">
							Schedule
						</a>
					</li>
					<li>
						<a href="/leaderboard">
							Leaderboard
						</a>
					</li> -->
					<li>
						<a href="/videos">
							Videos
						</a>
					</li>
					<!-- <li>
						<a href="#">
							Contests
						</a>
					</li> -->
					<!-- <li>
						<a href="/faqs" target="_top">
							FAQs
						</a>
					</li> -->
					<!-- <li>
						<a href="/vote" > Vote </a>
					</li> -->
				</ul>
				<!-- <div class="profile-icon enable-in-mobile enable-mobile-menu" style="opacity: 0">
					{#if menuMobile}
						{#if !$user.loggedOut}
							<a href="/" class="profile-btn" on:click={e => {
								User.logout();
							}}>
								<span class="material-icons">
									person
								</span>
								<strong>
									Logout
								</strong>
							</a>
						{:else}
							<a href="/" class="profile-btn">
								<strong class="mr-2 ml-0">
									Sign in
								</strong>
								<span class="material-icons">
									person
								</span>
							</a>
						{/if}
					{:else}
					<a href="#" class="profile-btn" class:active={!$user.loggedOut} on:click={()=>{ menuDropdown = !menuDropdown; return false; }}>
						<strong>
							{#if !$user.loggedOut}
							Hi, {$user.first_name} {$user.last_name}
							{:else}
							Sign in
							{/if}
						</strong>
						
						<span class="material-icons">
							person
						</span>
					</a>
					{/if}
					
				</div> -->
			</div>
			<!-- <div class="profile-icon" style="opacity: 0">
				{#if menuMobile}
					{#if !$user.loggedOut}
						<a href="/" class="profile-btn" on:click={e => {
							
							User.logout();
						}}>
							<span class="material-icons">
								person
							</span>
							<strong>
								Logout
							</strong>
						</a>
					{:else}
						<a href="/" class="profile-btn">
							<strong>
								Sign in
							</strong>
							<span class="material-icons">
								person
							</span>
						</a>
					{/if}
				{:else}
				<a href="#" class="profile-btn" class:active={!$user.loggedOut} on:click={()=>{ menuDropdown = !menuDropdown; return false; }}>
					<strong>
						{#if !$user.loggedOut}
						Hi, {$user.first_name} {$user.last_name}
						{:else}
						Sign in
						{/if}
					</strong>
					<span class="material-icons">
						person
					</span>
				</a>
				{/if}
				{#if menuDropdown}
					{#if $user.loggedOut}
						<div class="menu-dropdown">
							 <ul>
								<li>
									<a href="/" class="">
										Log in
									</a>
								</li>
							</ul> 
							
						</div>
					{:else}
						<div class="menu-dropdown">
							 <ul>
								<li>
									<a href="/" on:click={e => {
											User.logout();
										}}>
										Logout
									</a>
								</li>
							</ul> 
						</div>
					{/if}
					<UserMenu onClose={() => { menuDropdown = false }}/>
				{/if}
			</div> -->
		</div>
		
	</div>
</header>

<style>
</style>