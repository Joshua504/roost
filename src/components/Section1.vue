<template>
	<section class="banner">
		<div class="text-area">
			<h1>$ROOST</h1>
			<h3>HEY THERE I’M ROOST, CHAMPION OF THE BASE ECOSYTEM</h3>
			<label for="">CONTACT ADDRESS</label>
			<div class="input-area">
				<input type="text" />
				<button>copy</button>
			</div>
			<div class="btn-area">
				<button class="btn1">Buy $Roost</button>
				<button class="btn2">
					<img src="../assets/images/token_sdex.svg" alt="" />DEX TOOL
				</button>
				<img class="socials" src="../assets/images/socials.svg" alt="" />
			</div>
		</div>
		<div class="banner-img">
			<img src="../assets/images/Banner-img.svg" alt="" />
		</div>
	</section>
</template>

<script setup></script>

<style lang="scss" scoped>
@use "../styles/variables.scss" as *;
@use "../styles/mixin.scss" as *;
@use "sass:color" as color;

.banner {
	display: flex;
	justify-content: space-between;
	padding: 28px 118px;
	background: #fff6b5;
	height: 80vh;

	@include mobile {
		justify-content: center;
		flex-direction: column;
		height: auto;
		padding: 28px 15px;
		gap: 4rem;  
	}

	.text-area {
		width: 65%;

		@include mobile {
			width: 100%;
		}
		h1 {
			font: 400 200px "Font1";
			line-height: 151.06px;
			color: #3a80fe;
			margin-bottom: 50px;
			text-shadow: 2px 4px 4px #000000;

			@include mobile {
				font: 400 70px "Font1";
				line-height: 79.06px;
				margin-bottom: 27px;
				text-align: center;
			}
		}
		h3 {
			font: 400 64px Font1;
			line-height: 96.29px;
			color: #000000;
			margin-bottom: 56px;
			width: 95%;

			@include mobile {
				font: 400 22px "Font1";
				line-height: 31.06px;
				margin-bottom: 12px;
				text-align: center;
				width: 100%;
			}
		}
		label {
			font: 400 16px Font1;
			line-height: 24.14px;
			color: #c82347;
			margin-bottom: 20px;

			@include mobile {
				font: 400 16px "Font1";
				line-height: 24.06px;
				margin-bottom: 10px;
				text-align: center;
			}
		}

		.input-area {
			position: relative;
			width: 750px;
			margin-bottom: 56px;

			@include mobile {
				width: 100%;
				margin-bottom: 14px;
			}

			input {
				width: 100%;
				padding: 20px 100px 20px 25px;
				font: 700 16px Font3;
				border: 2px solid #000000;
				border-radius: 10px;
				outline: none;
				background: transparent;
				box-shadow: 0px 4px rgba(0, 0, 0, 0.6);
			}

			button {
				position: absolute;
				right: 10px;
				top: 50%;
				transform: translateY(-50%);
				padding: 15px 55px;
				border-radius: 10px;
				background: #ff9d46;
				border: 1px solid #000000;
				font: 700 16px Font3;
				line-height: 21.13px;
				color: #000000;
				text-transform: uppercase;
				box-shadow: 0px 2px rgba(0, 0, 0, 0.6);
				transition: all 0.3s ease-in-out;
				cursor: pointer;

				&:hover {
					box-shadow: 0px 0px rgba(0, 0, 0, 0.6);
					background: color.scale(#ff9d46, $lightness: -20%);
				}

				@include mobile {
					font: 400 14px "Font1";
					padding: 15px 20px;
				}
			}
		}

		.btn-area {
			width: 750px;
			display: flex;
			gap: 3em;
			position: relative;

			@include mobile {
				gap: 10px;
				width: 100%;
			}

			button {
				font: 400 25px Font3;
				text-transform: uppercase;
				width: 100%;
				padding: 20px 54px;
				border-radius: 10px;
				border: 2px solid #000000;
				box-shadow: 0px 4px rgba(0, 0, 0, 0.6);
				transition: all 0.3s ease-in-out;

				@include mobile {
					font: 400 14px "Font1";
					text-align: center;
					padding: 15px 20px;
					width: 100%;
				}
			}

			.btn1 {
				background: #3a80fe;
				color: #ffffff;

				&:hover {
					box-shadow: 0px 0px rgba(0, 0, 0, 0.6);
					background: color.scale(#508efe, $lightness: -20%);
				}
			}

			.btn2 {
				background: transparent;
				color: #000000;
				display: flex;
				justify-content: center;
				gap: 1.5em;
				align-items: center;

				&:hover {
					box-shadow: 0px 0px rgba(0, 0, 0, 0.6);
					background: #ff9d46;
				}
			}

			.socials {
				position: absolute;
				right: -15%;

				@include mobile {
					display: none;
				}
			}
		}
	}

	.banner-img {
		width: 35%;

		@include mobile {
			width: 100%;
		}
		img {
			width: 100%;
		}
	}
}
</style>
