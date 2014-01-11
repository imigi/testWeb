testWeb
=======

Android WebviewによるJavaScript連携のサンプル。



assetsフォルダにHTMLファイルを格納格納しておく
JavaScriptは、「_sample」がクラスオブジェクト名で
「outputLog」はメソッドです


<script type="text/javascript">
	function logout() {
		_sample.outputLog();
	}
	function vibrate() {
		_sample.vibrate(1000);
	}
</script>


Android 4.2 JavaScriptInterfaceへ公開するメソッド
次のアノテションを付加しなければならなくなった
要注意。
@JavascriptInterface
