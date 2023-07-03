//////////////////////////////////////////////////////////////
chức năng trênTạo() {
  Bánh mì nướng();
}
▬▬▬▬▬▬▬▬▬▬
     .TOAST
▬▬▬▬▬▬▬▬▬▬
Chức năng ShowToast() {
  var x = tài liệu.getElementById("Bánh mì nướng");
  x.className = "hiển thị";
  setTimeout(function(){ x.className = x.className.thay thế ("hiển thị", "");  }, 3900);
}
▬▬▬▬▬▬▬▬▬▬
     WEB FPS
▬▬▬▬▬▬▬▬▬▬
 var fps = tài liệu.getElementById ("khung hình / giây");

var startTime = Ngày.bây giờ();

khung var = 0;

đánh dấu chức năng() {

  var time = Ngày.bây giờ();

  khung++;

  if (time - startTime > 1000) {

      khung hình / giây.innerHTML = (khung / ((thời gian - startTime) / 1000)).toCố định(1);

      startTime = thời gian;

      khung = 0;

	}  cửa sổ.requestAnimationFrame(đánh dấu);

}

bét();

▬▬▬▬▬▬▬▬▬▬
     LIÊN KẾT
▬▬▬▬▬▬▬▬▬▬

Chức năng Youtube() {
  setTimeout(hàm() {
    cửa sổ.open('https://www.youtube.com/channel/UCiSP9FWliPIwG-w59dJdilQ', 'ultimate')},
  100);
}
chức năng Facebook() {
  setTimeout(hàm() {
    cửa sổ.open('https://www.facebook.com/100035052735014', 'ultimate')},
  100);
}
Chức năng Discord() {
  setTimeout(hàm() {
    cửa sổ.open('https://dsc.bio/WusThanhDieu', 'ultimate')},
  100);
}
Chức năng Telegram() {
  setTimeout(hàm() {
    cửa sổ.open('https://t.me/ThanhDieuChannel', 'ultimate')},
  100);
}

chức năng DarkMode() {
  phần tử var = tài liệu.thân thể;
  yếu tố.classList.Chuyển đổi ("Chế độ tối");
}
▬▬▬▬▬▬▬▬▬▬
   HOA ANH ĐÀO
▬▬▬▬▬▬▬▬▬▬

/*
var dừng, tĩnhx;
var img = Hình ảnh mới ();
img.src = "https://i.imgur.com/R9XUjfF.png";
 hàm Sakura(x, y, s, r, fn) {
				this.x = x;
				this.y = y;
				this.s = s;
				this.r = r;
 điều này.fn = fn;
			}
			Sakura.prototype.draw = function(cxt) {
				cxt.save();
				var xc = 40 * this.s / 4;
				cxt.translate(this.x, this.y);
				cxt.rotate(this.r);
 cxt.drawImage (img, 0, 0, 40 * this.s, 40 * this.s)
				cxt.restore();
			}
			Sakura.prototype.update = function() {
				this.x = this.fn.x(this.x, this.y);
				this.y = this.fn.y(this.y, this.y);
				this.r = this.fn.r(this.r);
				if(this.x > window.innerWidth ||
 điều này.x < 0 ||
					this.y > window.innerHeight ||
					this.y < 0
				) {
					this.r = getRandom('fnr');
 if(Math.random() > 0,4) {
						this.x = getRandom('x');
						this.y = 0;
						this.s = getRandom('s');
						this.r = getRandom('r');
					} else {
						this.x = window.innerWidth;
						this.y = getRandom('y');
						this.s = getRandom('s');
						this.r = getRandom('r');
					}
				}
			}
			SakuraList = function() {
				this.list = [];
			}
			SakuraList.prototype.push = function(sakura) {
 this.list.push (hoa anh đào);
			}
			SakuraList.prototype.update = function() {
				for(var i = 0, len = this.list.length; i < len; i++) {
					this.list[i].update();
				}
			}
			SakuraList.prototype.draw = function(cxt) {
				for(var i = 0, len = this.list.length; i < len; i++) {
					this.list[i].draw(cxt);
				}
			}
			SakuraList.prototype.get = function(i) {
 trả về this.list[i];
			}
			SakuraList.prototype.size = function() {
 trả về this.list.length;
			}
 hàm getRandom(option) {
 var ret, ngẫu nhiên;
 switch(tùy chọn) {
 Trường hợp 'X':
						ret = Math.random() * window.innerWidth;
 phá vỡ;
 Trường hợp 'Y':
						ret = Math.random() * window.innerHeight;
 phá vỡ;
 Trường hợp 's':
						ret = Math.random();
 phá vỡ;
 Trường hợp 'R':
						ret = Math.random() * 5;
 phá vỡ;
 Trường hợp 'FNX':
 ngẫu nhiên = -0,5 + Math.random() * 1;
 ret = hàm(x, y) {
 trả về x + 0, 5 * ngẫu nhiên - 1;
						};
 phá vỡ;
 Trường hợp 'FNY':
 ngẫu nhiên = 0,5 + Math.random() * 0,5
 ret = hàm(x, y) {
 trả về y + ngẫu nhiên;
						};
 phá vỡ;
 Trường hợp 'FNR':
 ngẫu nhiên = Math.random() * 0,01;
 ret = hàm(r) {
 trả về r + ngẫu nhiên;
						};
 phá vỡ;
				}
 trả lại;
			}
 hàm startSakura() {
				requestAnimationFrame = window.requestAnimationFrame ||
					window.mozRequestAnimationFrame ||
 window.webkitYêu cầuHoạt hìnhKhung ||
					window.msRequestAnimationFrame ||
					window.oRequestAnimationFrame;
				var canvas = document.createElement('canvas'),
 CXT;
 staticx = đúng;
				canvas.height = window.innerHeight;
				canvas.width = window.innerWidth;
				canvas.setAttribute('style', 'position: fixed;left: 0;top: 0;pointer-events: none;');
				canvas.setAttribute('id', 'canvas_sakura');
				document.getElementsByTagName('body')[0].appendChild(canvas);
				cxt = canvas.getContext('2d');
				var sakuraList = new SakuraList();
				for(var i = 0; i < 50; i++) {
					var sakura, randomX, randomY, randomS, randomR, randomFnx, randomFny;
					randomX = getRandom('x');
					randomY = getRandom('y');
					randomR = getRandom('r');
					randomS = getRandom('s');
					randomFnx = getRandom('fnx');
					randomFny = getRandom('fny');
					randomFnR = getRandom('fnr');
					sakura = new Sakura(randomX, randomY, randomS, randomR, {
						x: randomFnx,
						y: randomFny,
						r: randomFnR
					});
					sakura.draw(cxt);
					sakuraList.push(sakura);
				}
				stop = requestAnimationFrame(function() {
					cxt.clearRect(0, 0, canvas.width, canvas.height);
					sakuraList.update();
					sakuraList.draw(cxt);
					stop = requestAnimationFrame(arguments.callee);
				})
			}
			window.onresize = function() {
				var canvasSnow = document.getElementById('canvas_snow');
				canvasSnow.width = window.innerWidth;
				canvasSnow.height = window.innerHeight;
			}
			img.onload = function() {
				startSakura();
			}
 hàm stopp() {
 nếu(tĩnhx) {
 var con = document.getElementById("canvas_sakura");
 child.parentNode.removeChild (con);
 window.cancelAnimationFrame (dừng);
 staticx = sai;
				} else {
					startSakura();
				}
			}
		
		
*/
//////////////////////////////////////////////////////////////
