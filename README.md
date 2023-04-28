<!DOCTYPE html>
<html>
<head>
	<title>My Website</title>
	<style>
		header {
		  background-color: #800000;
		  color: #00B3B3;
		  text-align: center;
		  display: flex;
		  align-items: center;
		  justify-content: space-between;
		  padding: 20px;
		}	
		.logo span {
		  display: inline-block;
		  width: 0;
		  height: 0;
		  border-left: 45px solid transparent;
		  border-right: 45px solid transparent;
		  border-bottom: 90px solid #00B3B3;
		  text-align: center;
		  line-height: 50px;
		  font-weight: bold;
		  font-size: 28px;
		  color: #FFFFFF;
		  margin-left: -10px;
		  display: flex;
		  justify-content: center;
		  align-items: center;
		  transition: all 0.3s ease-in-out; /* Added */
		}
		
		.logo span:hover {
		  transform: rotate(180deg);
		}

		@media screen and (max-width: 768px) {
			header {
				flex-direction: column;
			}

			.logo {
				margin-bottom: 20px;
			}
		}
	</style>
</head>
<body>
  <header>
    <div class="logo">
      <span></span>LOFTIES</div> 
  </header>
</body>
</html>
