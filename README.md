
<!DOCTYPE html>
<html>
<head>
  <title>My Website</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    header {
      display: flex;
      align-items: center;
      background-color: #f2f2f2;
      padding: 10px;
    }

    header img {
      width: 60px;
      height: 60px;
      border-radius: 50%;
      margin-right: 15px;
    }

    header h1 {
      margin: 0;
      font-size: 22px;
    }

    .container {
      display: flex;
    }

    .sidebar {
      width: 200px;
      background-color: #ddd;
      padding: 15px;
      border-right: 2px solid black;
    }

    .sidebar a {
      display: block;
      margin: 8px 0;
      text-decoration: none;
      color: black;
      font-weight: bold;
    }

    .sidebar a:hover {
      color: blue;
    }

    .content {
      flex: 1;
      background-color: #eee;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <img src="wku.jpg" alt="User Picture">
    <div>
      <h1>NAME: ABDULMEJID KASSIM</h1>
      <p>ID: NSR/0010/16</p>
    </div>
  </header>

  <div class="container">
    <div class="sidebar">
      <h3>Labs & Assignments</h3>
      <a href="index.html">index</a>
      <a href="index2.html">index2</a>
      <a href="index3.html">index3</a>
      <a href="index4.html">index4</a>
      <a href="text.html.html">text</a>
      <a href="calculator.html">calculator</a>
      <a href="cell.html">cell</a>
    </div>

    <div class="content">
      <h2>My Profile</h2>
      <p>Hi I am Abdulmejid And This is my profile section. I am a student of Software engineering Department.</p>
    </div>
  </div>
<!-- Code injected by live-server -->
<script>
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
</script>
</body>
</html>
