<template>
	<v-app>
		<core-app-bar />
		<core-drawer />
		<core-view />
	</v-app>
</template>

<script>
import Drawer from '@/components/core/Drawer';
import AppBar from '@/components/core/AppBar';
import View from '@/components/core/View';
export default {
	props: {
		source: String,
	},
	data: () => ({
		drawer: null,
	}),
	components: {
		CoreDrawer: Drawer,
		CoreAppBar: AppBar,
		CoreView: View,
	},
};
</script>
