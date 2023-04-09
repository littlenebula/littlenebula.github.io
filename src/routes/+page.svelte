<main>
	<header>
		<aside>
			<img src="/logo.svg" alt="" width="192" height="257" />
			<span />
			<span />
			<span />
			<span />
		</aside>
		<h1>Little Nebula</h1>
	</header>

	<section>
    
  </section>

	<footer>&copy; 2023-present Little Nebula Pty Ltd.</footer>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
		min-height: 100vh;
	}

	header {
		padding: 4rem 0;
    width: 100%;
    overflow: hidden;
	}

	header aside {
		position: relative;
		z-index: 1;
    width: 100%;
	}

	header img {
    display: block;
    margin: auto;
		opacity: 0;
		animation: logo-appear-1 0.5s 0.5s ease-out forwards, logo-appear-2 0.3s 1s ease-in-out forwards;
	}
	@keyframes logo-appear-1 {
		0% {
			opacity: 0;
			transform: translateY(40%);
		}
		100% {
			opacity: 1;
			transform: translateY(-40%);
		}
	}
	@keyframes logo-appear-2 {
		0% {
			transform: translateY(-40%);
		}
		60% {
			transform: translateY(20%);
		}
		100% {
			transform: translateY(0);
		}
	}

	header span {
		position: absolute;
		bottom: 0;
		left: 50%;
		width: 91px;
		height: 87px;
		background: url(/star.svg) no-repeat;
	}

	header span:nth-of-type(1) {
		filter: invert(73%) sepia(98%) saturate(1534%) hue-rotate(1deg) brightness(106%) contrast(104%);
		opacity: 0;
		transform: translate(-100%, 50%);
		animation: star-1 0.4s cubic-bezier(0, 0.7, 0.38, 1) 0.5s forwards;
	}
	@keyframes star-1 {
		0% {
			opacity: 1;
			transform: translate(-100%, 50%);
		}
		50% {
			opacity: 1;
		}
		100% {
			opacity: 0;
			transform: scale(0.8) translate(-300%, 100%);
		}
	}

	header span:nth-of-type(2) {
		filter: invert(14%) sepia(96%) saturate(7493%) hue-rotate(339deg) brightness(103%)
			contrast(104%);
		opacity: 0;
		transform: scale(0.6) translate(-70%, 50%);
		animation: star-2 0.4s cubic-bezier(0, 0.7, 0.38, 1) 0.5s forwards;
	}
	@keyframes star-2 {
		0% {
			opacity: 1;
			transform: scale(0.6) translate(-70%, 50%);
		}
		50% {
			opacity: 1;
		}
		100% {
			opacity: 0;
			transform: scale(0.6) translate(-200%, 200%);
		}
	}

	header span:nth-of-type(3) {
		filter: invert(8%) sepia(73%) saturate(7449%) hue-rotate(305deg) brightness(94%) contrast(103%);
		opacity: 0;
		transform: scale(0.8) translate(-20%, 50%);
		animation: star-3 0.4s cubic-bezier(0, 0.7, 0.38, 1) 0.5s forwards;
	}
	@keyframes star-3 {
		0% {
			opacity: 1;
			transform: scale(0.8) translate(-20%, 50%);
		}
		50% {
			opacity: 1;
		}
		100% {
			opacity: 0;
			transform: scale(0.8) translate(100%, -10%);
		}
	}

	header span:nth-of-type(4) {
		filter: invert(14%) sepia(96%) saturate(7493%) hue-rotate(339deg) brightness(103%)
			contrast(104%);
		opacity: 0;
		transform: translate(0, 50%);
		animation: star-4 0.4s cubic-bezier(0, 0.7, 0.38, 1) 0.5s forwards;
	}
	@keyframes star-4 {
		0% {
			opacity: 1;
			transform: translate(0, 50%);
		}
		50% {
			opacity: 1;
		}
		100% {
			opacity: 0;
			transform: translate(250%, 100%);
		}
	}

	header h1 {
		opacity: 0;
		animation: text-appear 0.35s 1.1s ease-out forwards;
		position: relative;
		z-index: 0;
    text-align: center;
	}

	@keyframes text-appear {
		0% {
			opacity: 0;
			transform: translateY(-150%);
		}
		65% {
			opacity: 1;
			transform: translateY(100%);
		}
		100% {
			opacity: 1;
			transform: translateY(0);
		}
	}

	section {
		flex-grow: 1;
		height: 100%;
	}

	footer {
		color: #999;
		padding: 1rem;
	}
</style>
