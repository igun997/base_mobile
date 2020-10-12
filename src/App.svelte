<script>
	import { Router, Link, Route } from "svelte-routing"
	import Landing from "./Pages/Landing.svelte"
	export let url = "";
</script>
<style>
	@import "//stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css";
</style>
<nav class="navbar">
	<ul class="navbar-nav">
		<li class="nav-logo nav-item">
			<a href="#" class="nav-link">
				<span class="link-text">Quickly</span>
				<i class="link-icon fa fa-fw fa-angle-double-right"></i>
			</a>
		</li>
		<li class="nav-item active">
			<a href="#" class="nav-link">
				<i class="link-icon fa fa-fw fa-star"></i>
				<span class="link-text">Dashboard</span>
			</a>
		</li>
		<li class="nav-item">
			<a href="#" class="nav-link">
				<i class="link-icon fa fa-fw fa-bell"></i>
				<span class="link-text">Notification</span>
			</a>
		</li>
	</ul>
</nav>
<main>
	<Router url="{url}">
		<div>
			<Route path="/" component="{Landing}" />
		</div>
	</Router>

</main>