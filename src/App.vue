<template>
	<div id="app">
		<div class="wrapper clearfix">
			<player></player>

            <controls></controls>

			<dices></dices>
            
            <input type="number" placeholder="Final score" class="final-score">
            
            
        </div>
	</div>
</template>

<script>
import Player from './components/Player'
import Controls from './components/Controls'
import Dices from './components/Dices'
export default {
	name: 'app',
	data () {
		return {
			
		}
	},
	components: {
		Player,
		Controls,
		Dices
	}
}
</script>

<style>
	* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    
	}

	.clearfix::after {
		content: "";
		display: table;
		clear: both;
	}

	body {
		background-image: linear-gradient(rgba(62, 20, 20, 0.4), rgba(62, 20, 20, 0.4)), url(/public/assets/back.jpg);
		background-size: cover;
		background-position: center;
		font-family: Lato;
		font-weight: 300;
		position: relative;
		height: 100vh;
		color: #555;
	}

	.wrapper {
		width: 1000px;
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		background-color: #fff;
		box-shadow: 0px 10px 50px rgba(0, 0, 0, 0.3);
		overflow: hidden;
	}

</style>
