<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport"content="width=device-width, initial-scale=1"/>
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Flyteamtoy - Cửa hàng đồ chơi</title>
	<script src="icon/fontawesome/js/all.min.js"></script>
	<link rel="stylesheet" href="css/index.css">
	</head>
<body onload="createproduct();viewData1();checkDangNhap()">
	
	<div class="head">
		<div style="margin-left: 40px;">
			<img src="img/logo1.png">
			<img src="img/logo2.png">
		</div>
		<div class="search" >
				<input size="30px" type="" class="timkiem" id="timkiem" name="" placeholder="Các mẹ/bé cần mua gì ?" oninput="timkiemSanpham()">
				<button type="" style="font-size: 20px"><i class="fas fa-search" style="font-size: 25px;margin-left:-60px ;"></i></button>
		</div>

		<nav style="margin-right: 200px; font-size: 20px;display: flex;" >
			
			<a href="index.html" ><i class="fas fa-home"></i></a>
			<a href="index.html"><i class="fas fa-phone"></i></a>
			<div class="dropdown">
				<a href="" ><i class="fas fa-user-plus"></i></a>
				<div class="dropdown-content">
					<div id="loginaccount">
						<div><a href="html/dangnhap.html">Đăng nhập</a></div>
						<div><a href="html/dangki.html">Đăng ki</a></div>
					</div>
					<div id="accountUser" class="accountUser"></div>
				</div>
			</div>
			<a href="html/giohang.html"><i class="fas fa-shopping-cart"></i></a>
		</nav>
	</div>

		<div style="display: flex; margin-top: 5%;">
			<div class="left">
				<div class="first">
					<div style="margin-bottom: 10px;">
						<i class="fas fa-align-justify"></i><span style="font-size: 20px;margin-left: 10px;">Danh mục sản phẩm</span>
					</div>
					<nav class="left-nav">
						<a href="html/dogo.html" ><img src="img/nguago.png" alt="" > Tất cả</a>
						<a href="html/dochoimohinh.html" ><img src="img/robot.png" alt=""> Đồ chơi mô hình</a>
						<a href="html/dochoibupbe.html" ><img src="img/sosinh.png" alt="">Đồ chời búp bê</a>
						<a href="" ><img src="img/gau.png" alt="">Đồ chơi con trai</a>
						<a href="" ><img src="img/nha.png" alt="">Game điện tử</a>
						<a href="" ><img src="img/xe.png" alt="">Xe điều khiển</a>
					</nav>
				</div>
				<div class="second">
					<div class="camket">
						<div id="head"><span>3 cam kết bán hàng</span></div>
						<div style="display: flex;"><i class="far fa-calendar-check" style="color: orange; font-size: 30px; margin-right: 10px;"></i><span>Đồ chơi có mức giá tốt nhất thị trường, rẻ nhất so với chất lượng cam kết</span></div>
						<div style="display: flex;"><i class="far fa-calendar-check" style="color: orange; font-size: 30px;margin-right: 10px;"></i><span>Tư vấn bán hàng chi tiết, đưa ra lời khuyên tốt nhất cho cho mẹ</span></div>
						<div style="display: flex;"><i class="far fa-calendar-check" style="color: orange; font-size: 30px;margin-right: 10px;"></i><span>Bảo đảm đúng 100% chất liệu đồ chơi</span></div>
					</div>
				</div>
			</div>

			<div class="right">
				<div  class="danhmuc">
					<nav>
						<a href="index.html">Trang chủ</a>
						<a href="html/gioithieu.html">Giới thiệu</a>
						<a href="">Sản phẩm bán chạy</a>
						<a href="">Sản phẩm khuyễn mãi</a>
					</nav>
				</div>

				<div class="banner" id="bannerr">
					<div class="quangcao"></div>
					<div class="cham-tron">
						<a href=""><div class="cham cham1"></div></a>
						<a href=""><div class="cham cham2"></div></a>
						<a href=""><div class="cham cham3"></div></a>
					</div>
				</div>

				<div class="sanpham">
					<div class="sanpham-content"><span style="font-weight: bold; font-style: 20px;">Sản phẩm mới</span></div>

					<div class="machang" id="sanpham1"></div>
					<div class="machang" id="sanpham2"></div>
					<div class="machang" id="sanpham3"></div>
					<div class="machang" id="sanpham4"></div>
					
					<div>
						<div class="cham-tron" style="padding-bottom: 20px;">
							<button id="page-1" onclick="viewData1()">1</button>
							<button id="page-2" onclick="viewData2()">2</button>
							<button id="page-3" onclick="viewData3()">3</button>
							<button id="page-4" onclick="viewData4()">4</button>
						</div>
					</div>
				</div>

			</div>
		</div>	
		<div class="footer">
			<div style="display: flex;justify-content: space-around;">
				<p>Câu hỏi thường gặp</p>
				<p>Chính sách bảo mật</p>
				<p>Chính sách đổi trả</p>
				<p>Giao hàng</p>
				<p>Hướng dẫn mua hàng</p>
			</div>
			<div>
				<div style="text-align: center;">
					<p>Địa chỉ shop: 275 An Dương Vương, Phường 03, Quận 05	, TP. Hồ Chí Minh</p>
					<p>Điện thoại: 0979 08 6789</p>
				</div>
				<div style="text-align: center;">
					<img src="img/logo1.png" alt="" style="height: 50px;">
					<img src="img/logo2.png" alt="" style="height: 50px;">
				</div>
				<div style="text-align: center;font-size: 30px; padding: 10px;">
					<a href="https://www.facebook.com/	"><i class="fab fa-facebook" style="color: white;"></i></a>
					<a href="https://www.youtube.com/"><i class="fab fa-youtube"  style="color: white;"></i></a>			
					<a href="https://www.instagram.com/"><i class="fab fa-instagram"  style="color: white;"></i></a>
				</div>
				<div style="text-align: center;">
					<p>Copyright © 2015-2016 by Dochoitreem.com - All rights reserved.</p>
					<p>Công ty cổ phần Yêu Trẻ chuyên kinh doanh buôn bán sỉ và lẻ các loại đồ chơi, đồ chơi trẻ em, đồ chơi cho bé, đồ chơi trẻ em an toàn như: búp bê, đất nặn, xe điều khiển từ xa.</p>
				</div>
			</div>
		</div>
</body>
<script src="js/data.js"></script>
</html>
