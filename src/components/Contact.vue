<template lang="pug">
.contactFlex
	.contactList(v-for="item in list")
		.contactApp {{item.title}}
		.contactSlash {{item.slash}}
</template>

<script>
export default {
	name: 'Contact',
	props: {
		msg: String
	},
	data(){
		return{
			list:[
				{title:'Facebook', slash:'|'},
				{title:'Twitter', slash:'|'},
				{title:'Email'}
			]
		}
	}
}
</script>

<style lang="sass">
.contactFlex
	display: flex
	flex-direction: row
	// border: 1px solid red
	justify-content: space-between
	position: absolute
	width: 402px
	height: 45.12px
	right: 120px
	top: 45px

.contactList
	// border: 1px solid blue
	width: 1340px
	height: 45px
	display: flex
	flex-direction: row

.contactApp
	//border: 1px solid orange
	width: 115px
	height: 45px
	font-style: normal
	font-weight: normal
	font-size: 30px
	line-height: 45px
	color: white

.contactSlash
	// border: 1px solid green
	width: 38.12px
	height: 45.12px
	right: 100px
	top: 45px
	font-size: 25px
	font-weight: bold
	line-height: 45px
	color: grey
</style>