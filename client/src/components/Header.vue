<template>
	<div>
		<div class="">
			<ul class="topnav">
				<li><router-link :to="{ name: 'cats' }" class="font">Cat Food</router-link></li>
				<li><router-link :to="{ name: 'users' }" class="size">Users</router-link></li>
				<li><router-link :to="{ name: 'login' }" class="size">Login</router-link></li>
			</ul>
			<div class="clearfix" />
		</div>	
	</div>
</template>
<script>
export default {};
</script>
<style scoped>
ul.topnav {
  list-style-type: none;
  margin-top: -60px;
  padding: 0;
  overflow: hidden;
  /* เปลี่ยนสี navbar */
  background-color: #333;
}

ul.topnav li {float: left;}

ul.topnav li a {
  display: block;
  /* เปลี่ยนสี font */
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

ul.topnav li a:hover:not(.active) {background-color: #111;}

ul.topnav li a.active {background-color: #04AA6D;}

ul.topnav li.right {float: right;}

@media screen and (max-width: 600px) {
  ul.topnav li.right, 
  ul.topnav li {float: none;}
}
.clearfix {
	clear: left;
}
.font {
	font-size: 20px;
}
.size
{
	font-size: 15px;
	margin-top: 5px;
}
.log{
	margin-right: 5px;
}
</style>
