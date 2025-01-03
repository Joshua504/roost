<template>
	<nav>
		<div>
			<router-link to="/"
				><img src="../assets/images/Logo.svg" alt=""
			/></router-link>
		</div>
		<ul>
			<router-link class="link">
				<li>home</li>
			</router-link>
			<router-link class="link">
				<li>about us</li>
			</router-link>
			<router-link class="link">
				<li>roadmap</li>
			</router-link>
			<router-link class="link">
				<li>tokenomics</li>
			</router-link>
			<router-link class="link">
				<li>join community</li>
			</router-link>
		</ul>
		<div><button>presale</button></div>
	</nav>
</template>

<script setup></script>

<style lang="scss">
@use "../styles/variables.scss" as *;
@use 'sass:color' as color;

nav {
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding: 28px 118px;
	background: #fff6b5;

	ul {
		display: flex;
		gap: 22px;
		align-items: center;

		.link {
			text-decoration: none;

			li {
				list-style: none;
				text-transform: capitalize;
				font: 700 16px Font3;
				color: #000000;
			}
		}
	}

	button {
		padding: 10px 22px;
		font: 700 16px Font3;
		color: #ffffff;
		text-transform: uppercase;
		outline: transparent;
		border: 2px solid #000000;
		border-radius: 10px;
		background: #508efe;
		cursor: pointer;
		box-shadow: 0px 4px rgba(0, 0, 0, 0.6);
    transition: all 0.3s ease-in-out;

		&:hover {
			box-shadow: 0px 0px rgba(0, 0, 0, 0.6);
			background: color.scale(#508efe, $lightness: -20%);
		}
	}
}
</style>
