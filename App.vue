<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
			// #ifdef APP-PLUS-NVUE
			const domModule = weex.requireModule('dom')
			domModule.addRule('fontFace', {
				'fontFamily': "iconfont",
				'src': "url('https://at.alicdn.com/t/font_1365296_vumpzwvr0z.ttf')"
			});
			// #endif
			
			
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/*每个页面公共css */
	@import url("./common/free.css");
	@import url("./common/common.css");
	/* #ifndef APP-PLUS-NVUE */
	@import url("./common/free-icon.css");
	/* #endif */
</style>
