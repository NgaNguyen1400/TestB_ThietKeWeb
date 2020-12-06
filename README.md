# Thiết kế website


<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cool Summer</title>
    <link rel="StyleSheet" href="./css/style.css">

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>

</head>
<style>
	
</style>

<body>
    <header>
		<div class="row" style="max-width:5000px;margin-top:0px">
		<img src="" ></a>
        <h1>SUMMER</h1>
        </div>
     
            
    
    </header>
    <nav >
		<div style="text-align:center">
        <ul>
			
            <li><a data-section="home" class="active">TRANG CHỦ </a></li>
            <li><a data-section="services">GIỚI THIỆU</a></li>
            <li class="dropdown">
                <a href="javascript:void(0)" class="dropbtn">SẢN PHẨM</a>
                <div class="dropdown-content">
                    <a data-section="link1">Áo thun</a>
                    <a data-section="link2">Váy công sở</a>
					<a data-section="link3">Váy dạ hội</a>
					<a data-section="link3">Váy dạ hội</a>
                </div>
            </li>
            <li ><a data-section="about">LIÊN HỆ</a></li>
		</ul>
	</div>
    </nav>

    <section id="home" class="hideable-section">
       <div class="row" >
		  <p style="text-align: center;">SẢN PHẨM BÁN CHẠY NHẤT</p>
		  <div class="col-3">
			  <a href=""><img src="images/orange.jpg"></a>
			  <p>Giày convert cao cổ tim</p>
			  <div class="cost"><span>600.000 <u>đ</u></span></div>
			  <a href="#"><button class="">Thêm vào giỏ</button></a>
		  </div>
		  <div class="col-3">
			<a href=""><img src="images/orange.jpg"></a>
			<p>Giày convert cao cổ tim</p>
			<div class="cost"><span>600.000 <u>đ</u></span></div>
			<a href="#"><button class="">Thêm vào giỏ</button></a>
		  </div>
		   <div class="col-3">
			<a href=""><img src="images/orange.jpg"></a>
			<p>Giày convert cao cổ tim</p>
			<div class="cost"><span>600.000 <u>đ</u></span></div>
			<a href="#"><button class="">Thêm vào giỏ</button></a>
		</div>
		<div class="col-3">
			<a href=""><img src="images/orange.jpg"></a>
			<p>Giày convert cao cổ tim</p>
			<div class="cost"><span>600.000 <u>đ</u></span></div>
			<a href="#"><button class="">Thêm vào giỏ</button></a>
		</div>
		  
	   </div> 

	
	<hr class="my-4">
    </section>

    <section id="services" class="hideable-section">
        <div>Services content</div>
    </section>

    <section id="about" class="hideable-section">
        <div>About content</div>
    </section>

    <section id="link1" class="hideable-section">
        <div>Link1 content</div>
    </section>

    <section id="link2" class="hideable-section">
        <div>Link2 content</div>
    </section>

    <section id="link3" class="hideable-section">
        <div>Link3 content</div>
    </section>

    <script>
        $(function() {
            $('nav ul li a').click(function() {
                // Lấy section để hiển thị
                var $section = $('#' + $(this).data('section'));

                // Nếu đang hiện thì không làm gì.
                // Nếu không, ẩn tất cả các se cho hiện (kiểu fade in) phần mong muốn.
                if (!$section.is(':visible')) {
                    $('.hideable-section').hide();
                    $section.fadeIn();
                }
            });
        });
    </script>
</body>

</html>
