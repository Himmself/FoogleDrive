<script>
	import { AppBar, Button, Icon, Menu, ListItem, MaterialApp, TextField } from 'svelte-materialify';
	import { mdiMenu, mdiDotsVertical, mdiMagnify, mdiCogOutline } from '@mdi/js';
  </script>

<MaterialApp>
	<div style="position:relative;height:250px">
		<AppBar>
			<img src="https://upload.wikimedia.org/wikipedia/commons/d/da/Google_Drive_logo.png" alt="Google Drive Logo"
					class="logo">
			<h4 class="appTitle">SeanDrive</h4>
			<div id="searchBar">
				<TextField filled dense rounded >
					<div slot="prepend">
        				<Icon path={mdiMagnify} />
      				</div>
	  				Search in Drive
				</TextField>
			</div>
			<div id="appBarButtons">
				<Button icon>
					<Icon path={mdiCogOutline} />
				</Button>
			</div>
		</AppBar>
	</div>
	<!-- <AppBar>
	  <div slot="icon">
		<Button fab depressed>
		  <Icon path={mdiMenu} />
		</Button>
	  </div>
	  <span slot="title">Title</span>
	  <div style="flex-grow:1" />
	  <Button>Item</Button>
	  <Menu right>
		<div slot="activator">
		  <Button fab depressed>
			<Icon path={mdiDotsVertical} />
		  </Button>
		</div>
		<ListItem>Item 1</ListItem>
		<ListItem>Item 2</ListItem>
		<ListItem>Item 3</ListItem>
	  </Menu>
	</AppBar> -->
	</MaterialApp>


<style>
	.logo{
		height: 100%;
		/* width: 100%; */
		object-fit: contain;
	}
	.appTitle{
		color: rgb(85, 81, 81);
		margin: 12px;
		font-size: 25px;
	}
	#searchBar{
		margin-left: 10%;
		margin-right: 25%;
		width: 50%;
	}
	#appBarButtons{
		margin-right: 10px;
		margin-top: auto;
	}
</style>