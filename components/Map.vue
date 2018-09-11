<template>
	<div>
		<div id="map"></div>
	</div>
</template>

<script>
	export default {
    data() {
        return {

        }
    },
    mounted: function() {
        this.initMap();
},
    methods: {
        initMap: function() {
            this.map = new google.maps.Map(document.getElementById('map'), {
            center: {lat: 83.9207, lng: 35.9565},
            scrollwheel: false,
            zoom: 4
            })
        }
    }
}
</script>

<style>
	#map {height:300px;width:500px;}
</style>