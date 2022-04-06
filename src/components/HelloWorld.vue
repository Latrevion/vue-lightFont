
<template>

  <div class="hello">
		<span style="--style:1">L</span>
		<span style="--style:2">a</span>
		<span style="--style:3">t</span>
		<span style="--style:4">r</span>
		<span style="--style:5">e</span>
		<span style="--style:6">v</span>
		<span style="--style:7">i</span>
		<span style="--style:8">o</span>
		<span style="--style:9">n</span>
 </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
       
        .hello{
            position: relative;
            top: 200px;
            font: 900 100px '';
            color: #333;
            cursor: pointer;
			letter-spacing: 5px;
        }
        .hello span{
            transition: .5s;
            transition-delay: calc(var(--style)*.1s);
        }
        .hello:hover span{
            color: #fff;
            text-shadow: 0 0 10px #fff,
            0 0 20px #fff,
            0 0 30px #fff,
            0 0 50px #fff,
            0 0 80px #fff;
        }

</style>
