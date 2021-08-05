<script>
 	import Format from '../layouts/partials/Format.svelte';
	import { Tabs, TabList, TabPanel, Tab } from '../components/tabs/tabs.js';
	import Video from '../components/Video.svelte';
</script>
<div class="format-page">
	<div class="top-section">
		<h1 class="title">Format</h1>
		<Video url="https://www.youtube.com/watch?v=obJ469oN0Vg" thumb="/images/day_13_conquest_format-explainer_thumb_HINDI.jpg"/>
		<div class="format-details">
			<Format />
		</div>
	</div>
</div>
<Tabs>
	<TabList>
		<Tab>Registrations</Tab>
		<Tab>In-game qualifiers</Tab>
		<Tab>Online Playoffs</Tab>
		<Tab>League Stage</Tab>
		<Tab active={true}>Grand Finals</Tab>
	</TabList>
	<TabPanel>
		<div class="container">
			<!-- <div class="video-thumb mt-40">
				<div class="video-thumbnail">
					<div class="shadow-layer"></div>
					<img src="images/video-thumb.jpg" alt="video">
					<a href="#" class="play-btn">
						<span class="material-icons">
							play_arrow
						</span>
					</a>
					<div class="video-info">
						<h6>
							Qualcomm Snapdragon® Conquest
							Season 1 - Trailer
						</h6>
						<span class="date-txt">
							12 October 2020. 00:57 sec
						</span>
					</div>
				</div>
			</div> -->
			<section class="process-content">
				<div class="container">
					<div class="row mt-40 pb-4">
						<div class="col-md-6">
							<h3 class="col-heading">HOW TO REGISTER?</h3>
							<p class="col-paragraph">
								To register for Qualcomm(R) Snapdragon Conquest(TM): Free Fire Open 2020, all you need to do is click Register Now, provide your details and follow the steps. Once you have registered your account, you can join a Squad or create your own, with a total of 4 members.
							</p>
							<h3 class="col-heading">JOINING A SQUAD</h3>
							<p class="col-paragraph">
								To join a squad, enter the team code provide by the Team Leader. You can also search for the Squad ID or the Team Leader’s name for the squad you wish to join and click on ‘Join Squad’. Your request to join will be completed as soon as the leader of the squad accepts it.
							</p>
						</div>
						<div class="col-md-6">
							<h3 class="col-heading">CREATING A SQUAD</h3>
							<p class="col-paragraph">
								Type in your team name and click on the Create Squad button to create your squad. You can now invite your friends by sending them the invite code or link. Once your squad has 4 members, you are all set to go! Time to practice and battle it out for glory! 
							</p>
						</div>
					</div>
				</div>
			</section>
		</div>
	</TabPanel>
	<TabPanel>
		<div class="container">
			<section class="process-content">
				<div class="container">
					<div class="row mt-40 pb-4">
						<div class="col-md-12 col-sm-12 col-xs-12 col-lg-12">
							<p class="col-paragraph">
								The In-game qualifiers will begin soon after the registration ends. During this phase all registered players are required to form a squad with their registered teammates in the Free Fire game app and play at least 15 classic matches. The scores of your 10 best matches will be picked for ranking purposes. The top 648 teams will progress to the next round. Ensure you play all the required matches with your registered teammates during this time!
							</p>
							<Video url="https://www.youtube.com/watch?v=LjSX7wYgx4o" thumb="/images/day28_YT_howtoplay_thumb.jpg"/>
						</div>
					</div>
				</div>
			</section>
		</div>
	</TabPanel>
	<TabPanel>
		<div class="container">
			<section class="process-content">
				<div class="container">
					<div class="row mt-40 pb-4">
						<div class="col-md-12 col-sm-12 col-xs-12 col-lg-12">
							<p class="col-paragraph">
								Once the in-game qualifiers have ended, the 648 qualifying teams will be seeded into 54 groups. There will be 3 rounds of elimination in the Playoffs as follows
							</p>
							<div class="table-responsive">
								<div class="table-section">
									<table class="table">
										<thead>
											<tr>
												<th scope="col">Round</th>
												<th scope="col">Teams</th>
												<th scope="col">Groups</th>
												<th scope="col">Format</th>
												<th scope="col">No. of Matches</th>
												<th scope="col">Qualifying Teams</th>
											</tr>
										</thead>
										<tbody>
											<tr>
												<td>Playoffs - Round 1</td>
												<td>648 Teams</td>
												<td>54 Groups</td>
												<td>Single Elimination, Best of 1</td>
												<td>54 Matches</td>
												<td>216 – Top 4 from each group</td>
											</tr>
											<tr>
												<td>Playoffs - Round 2</td>
												<td>216 Teams</td>
												<td>18 Groups</td>
												<td>Single Elimination, Best of 1</td>
												<td>18 Matches</td>
												<td>72 – Top 4 from each group</td>
											</tr>
											<tr>
												<td>Playoffs - Round 3</td>
												<td>72 Teams</td>
												<td>6 Groups</td>
												<td>Single Elimination, Best of 3</td>
												<td>18 Matches</td>
												<td>18– Top 3 from each group</td>
											</tr>
										</tbody>
									</table>
								</div>
							</div>
						</div>
					</div>
				</div>
			</section>
		</div>
	</TabPanel>
	<TabPanel>
		<div class="container">
			<section class="process-content">
				<div class="container">
					<div class="row mt-40 pb-4">
						<div class="col-md-12 col-sm-12 col-xs-12 col-lg-12">
							<p class="col-paragraph">
								This is where the competition is going to get a lot more fierce! The 18 teams qualifying from the Playoffs and 6 invited teams will now battle it out across a month-long league style format. The 24 teams will be seeded into 4 groups and will play 24 matches, round robin format, best of 4 rounds every week for 4 weeks. The top 12 performing teams at the end of week 4 will move onto the grand finals!
							</p>
							<p class="col-paragraph">
								These matches are going to be a high-level & action packed, it would probably a good time to use those pro-strats of your squad!
							</p>
						</div>
					</div>
				</div>
			</section>
		</div>
	</TabPanel>
	<TabPanel active={true}>
		<div class="container">
			<section class="process-content">
				<div class="container">
					<div class="row mt-40 pb-4">
						<div class="col-md-12 col-sm-12 col-xs-12 col-lg-12">
							<p class="col-paragraph">
								The Grand Finals will be held across 2 days as we witness the best teams in the scene battle it out for the chance to be the inaugural champions! The 12 qualifying teams will play 12 matches, 6 matches per day and the team with the highest cumulative score will be Free Fire Open Champions 2020!
							</p>
						</div>
					</div>
				</div>
			</section>
		</div>
	</TabPanel>
</Tabs>
<style>
	.title {
		font-size: 42px;
		font-family: 'Qualcomm Next Medium';
		margin-bottom: 0;
		text-align: center;
		letter-spacing: 0;
		color: #ffffff;
		padding: 80px 0 40px 0;
	}

	.btn-section {
		padding-top: 50px;
	}

	.col-heading {
		font-size: 16px;
		font-family: "Qualcomm Next Medium";
		font-stretch: normal;
		font-style: normal;
		line-height: 1.5;
		letter-spacing: normal;
		letter-spacing: 0;
		color: #0b2742;
	}

	.col-paragraph {
		font-size: 16px;
		line-height: 24px;
		font-weight: normal;
		font-stretch: normal;
		font-style: normal;
		letter-spacing: normal;
		letter-spacing: 0;
		color: #0b2742;
		margin-bottom: 2rem;
	}

	.register-btn {
		width: 300px;
		text-decoration: none;
		margin-bottom: 20px;
		border-radius: 25px;
		font-size: 16px;
		font-family: "Qualcomm Next Medium";
		font-stretch: normal;
		font-style: normal;
		letter-spacing: normal;
		text-align: center;
		display: inline-block;
		background-color: #ffffff;
		color: #3253dc;
		border: none;
	}

	.register-text {
		font-size: 16px;
		color: #ffffff;
		font-weight: normal;
		font-stretch: normal;
		font-style: normal;
		line-height: normal;
		letter-spacing: normal;
		text-align: center;
	}

	.register-text a {
		font-family: "Qualcomm Next Medium";
		color: #ffffff;
		text-decoration: none;
	}
</style>