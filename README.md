# HTML5/CSS3 - Elemento Centralizado

Centraliza qualquer elemento independente do dispositivo, elemento ou resolução.


## Arquivos

### .html

	<!DOCTYPE html>
	<html lang="pt">

	<head>
		<meta charset="UTF-8">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<meta http-equiv="X-UA-Compatible" content="ie=edge">
		<link rel="stylesheet" href="style.css">
		<title>Input Customizado</title>
	</head>

	<body>
		<div class="container">
			<form action="">
				<h2><img src="./img/logo.png" alt="google"></h2>
				<input type="text" placeholder="Pesquise no Google ou digite a URL">
				<buttton class="btn">Pesquisar</buttton>
			</form>
		</div>
	</body>

	</html>

### .css
Destaque para os elementos sinalizados com as setas:

	body {
		margin: 0;
		padding: 0;
		width: 100%;
		height: 100vh;
		background-color: white;
		display: table;
		font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
	}

	.container {
		position: absolute;
		top: 50%;
		left: 50%;
		padding: 0;
		transform: translateX(-50%) translateY(-50%);
	}

	h2 {
		text-align: center;
		margin: 0;
		padding: 0;
	}

	img {
		text-align: center;
		width: 50%;
		margin: 0;
		padding: 0;
	}

	input { <--
		/* display: block; */
		width: 100%;
		height: 50px;
		border: 1px solid #cccccc;
		border-radius: 3px;
		outline: none;
		margin: 0 auto;
		margin-top: 24px;
		padding: 0 16px;
		font-size: 100%;
		-webkit-box-shadow: 0px 3px 3px 0px rgba(204, 204, 204, 1);
		-moz-box-shadow: 0px 3px 3px 0px rgba(204, 204, 204, 1);
		box-shadow: 0px 3px 3px 0px rgba(204, 204, 204, 1);
	}

	input:hover,
	input:visited {
		-webkit-box-shadow: 0px 3px 10px 0px rgba(204, 204, 204, 1);
		-moz-box-shadow: 0px 3px 10px 0px rgba(204, 204, 204, 1);
		box-shadow: 0px 3px 10px 0px rgba(204, 204, 204, 1);
	}

	::placeholder {
		/* Chrome, Firefox, Opera, Safari 10.1+ */
		color: #666;
		opacity: 0.7;
	}

	:-ms-input-placeholder {
		/* Internet Explorer 10-11 */
		color: #666;
		opacity: 0.7;
	}

	::-ms-input-placeholder {
		/* Microsoft Edge */
		color: #666;
		opacity: 0.7;
	}

	.btn {
		cursor: pointer;
		display: block;
		max-width: 120px;
		max-height: 53px;
		margin: 0 auto;
		margin-top: 24px;
		padding: 10px 16px;
		color: white;
		text-align: center;
		text-transform: uppercase;
		background-color: #304ffe;
		border-radius: 3px;
		border: none;
		border-bottom: 3px solid #0026ca;
	}

	.btn:active {
		background-color: #0026ca;
		border-bottom-color: #304ffe;
	}

