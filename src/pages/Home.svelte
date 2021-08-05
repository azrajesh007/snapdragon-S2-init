<script>
	import Format from '../layouts/partials/Format.svelte';
	import {User} from '../models/user';
	import Video from '../components/Video.svelte';
	import Vote from '../pages/vote.svelte'
	import Insider from '../layouts/partials/Insider.svelte';
	const user = User.getUser();

	const urlParams = new URLSearchParams(window.location.search);
	if(urlParams.get('r') != null){
		window.localStorage.setItem('referral', urlParams.get('r'));
	}
</script>
<section class="main-section">
	<div class="container-fluid">
		<div class="row">
			<div class="col-lg-5 col-sm-5 col-xs-12">
				<!-- <div class="game-pic"></div> -->
				<div class="content-wrapper s2-title-section">
					<div class="qual-banner-logo">
						<img src="images/home-logo.png" alt="home-logo">
					</div>
					<div class="free-fire-block">
						<div class="winnig-price">
							<div class="winner-label pt-3">
								SEASON 2
							</div>
							<div class="price-txt">
								COMING SOON
							</div>
						</div>
					</div>
					
					<div class="banner-bttom mt-40">
						<a href="#" class="btn btn-primary register-btn watch-finals-btn">
							Watch Trailer
						</a>
					</div>
					<div class="free-fire-logo">
						<img src="images/logos-sponsor.png" alt="FreeFire-Logo">
					</div>
				</div>
				<!-- <div class="game-pic game-pic-right"></div> -->
			</div>
			<div class="col-lg-7 col-sm-7 col-xs-12 p-0">
				<div class="hero-image">
					<img src="images/hero-charector.png" alt="home-logo">
				</div>
			</div>
		</div>
	</div>
</section>
<!-- <section class="social-links-top">
	<div class="container text-center">
		<h6>Follow us on</h6>
		<ul>
			<li>
				<a href="https://www.facebook.com/snapdragonconquest/" target="_blank">
					<img src="images/ic-facebook.png" alt="Facebook">
				</a>
			</li>
			<li>
				<a href="https://www.instagram.com/snapdragonconquest/" target="_blank">
					<img src="images/ic-instagram.png" alt="Instagram">
				</a>
			</li>
			<li>
				<a href="https://mobile.twitter.com/_ConquestEsport" target="_blank">
					<img src="images/twitter.png" alt="Twitter">
				</a>
			</li>
			<li>
				<a href="https://youtube.com/channel/UCqfsjVyKK2_ajIgG_HqR36w" target="_blank">
					<img src="images/ic-youtube.png" alt="Youtube">
				</a>
			</li>
		</ul>
	</div>
</section> -->
<!-- voting  section -->
<Insider />
<!-- voting section -->

<style>
	.winnig-price {
		position: relative;
		padding-bottom: 1em;
	}

	.winnig-price:before, .winnig-price::after  {
		    content: "";
			position: absolute;
			height: 1px;
			width: 20%;
			border-bottom: 1px solid #cecece;
			left: 50%;
			transform: translateX(-50%);
			top: 0;
		}

		.winnig-price::after {
			bottom: 0;
			top: 100%;
		}
</style>