<html>
	<head>
	<meta content="text/html; charset=euc-kr">
		<style type="text/css">
		</style>
		<script src="https://code.jquery.com/jquery-3.6.1.js"></script>
		<script type="text/javascript" language="javascript">
			$( document ).ready(function() {
				reflashText();
				
			});
			
			var divClickFlg = false;
			function dispClick(obj)
			{
				if(obj.tagName == "DIV")
				{
					if(divClickFlg)
					{
						divClickFlg = false;
					}
					else
					{
						reflashText();
					}
				}
				else
				{
					divClickFlg = true;
					var beforeColor = $(obj).css("color");
					beforeColor = rgbToHex(beforeColor);
	
					if(beforeColor == "#ffffff")
					{
						$("span").each(function (i, item)
						{
							var afterColor = $(item).attr("tcolor");
							$(item).css("color", afterColor);
						});
					}
					else
					{
						$("span").each(function (i, item)
						{
							if(beforeColor != rgbToHex($(item).css("color")))
							{
								$(item).css("color", "#ffffff");
							}
							else
							{
								var afterColor = $(item).css("color");
								$("#showText").html($("#showText").html() + " " + $(item).html());
								$("#showText").css("color", afterColor);
								$(item).css("color", "#ffffff");
							}
						});
					}
				}
			}
			
			function reflashText()
			{
				var windowWidth = window.innerWidth / 2;
				var windowHeight = window.innerHeight;
				
				$("#showText").html("");
				$("#showText").css("color",  "#ffffff");
				
				$("#divArea").attr("style","width:"+  windowWidth +";height:"+windowHeight+";");
				
				$("span").each(function (i, item)
				{
					$(item).attr("style", "position:relative;left:"+Math.floor(Math.random() * windowWidth)+";top:"+Math.floor(Math.random() * windowHeight)+";");
					
					var afterColor = $(item).attr("tcolor");
					$(item).css("color", afterColor);
				});
			}
			
			function rgbToHex(beforeColor) {
			
				var beforeColorArr = beforeColor.toString().replace("rgb", "").replace("(", "").replace(")", "").split(",");
				r = parseInt(beforeColorArr[0], 10);
				g = parseInt(beforeColorArr[1], 10);
				b = parseInt(beforeColorArr[2], 10);
			  
				return "#" + (1 << 24 | r << 16 | g << 8 | b).toString(16).slice(1);
			}
			
		</script>
		
		
	</head>
	<body id="bodyTag">
		<div id="showText"></div>
		<div id="divArea" onclick="dispClick(this);">
		<span style="color:black" onclick="dispClick(this);" tcolor="black">코 성형했다가 부작용이</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">심하게 와서 난리 났대</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">벌레 같은 놈들 언젠간 저럴 줄 알았지.</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">그 사람이 이상한 흰 가루를</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">가지고 있는 걸 봤어.</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">마약이 아닐까? 신고해.</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">그 사람 그 자리에서 당장 죽으라고 </span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">소리치면서 울었다는 거야.</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">그 유명 방송인 소문 들었어?</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">진짜 장난 아니던데</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">완전 나쁜 새끼들이야.</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">그 자식 날 완전히 개무시하더니 그 꼴 난 거잖아.</span>
		<span style="color:black"onclick="dispClick(this);" tcolor="black">아무래도 수상한 거 같지 않아?</span>




		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">2007년 3월 20일 화</span>
		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">토티리스=포티리스</span>
		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">캐롯아? 넌 지구평화를 위해 (편지)</span>
		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">싸우니? 너는로봇이잖아.디가 우리다</span>
		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">사는 지구에오면 무슨 일을 할거니? </span>
		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">삼x람을 도와주는일 난 네가 TV에서</span>
		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">싸우는 장면이 재일 잼있는데</span>
		<span style="color:#F23D4C"onclick="dispClick(this);" tcolor="#F23D4C">이젠 너의 만화 많이볼께</span>



		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">2007년 4월 2일 월</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">난 이책을 읽고나서 멸종된 새도</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">있다는걸 알게되었다 동물을 잘알아는데</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">새는좀 모르겠다 그리고 지구상에있는</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">새중에서 (유타조같은거 뺴고)</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">콘드로라는 새가있다 날개를 펼치면 3m</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">이상이된다 내가 제일좋아하는새는</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">흰머리독수리다 왜냐하면 사냥을</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">할때 집중하는게 멋있기 때문이다.</span>
		<span style="color:#55CCD9"onclick="dispClick(this);" tcolor="#55CCD9">나도이제 공부할때 집중을많이해야겠다</span>


		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">2007년 4월 22일</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">아마존에서 살아남기</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">레오에게</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">레오야 넌 장난은 많이 치는데 나랑</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">똑같다 넌 무인도에서도 살아 남았잖아.</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">정말운이 좋구나 나도 이책 을읽고나서 아마존</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">에가치면 이것첨럼 따라할꺼야</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">레오야 몸건강하고 밥 잘먹어 안녕!</span>
		<span style="color:#4C85D8"onclick="dispClick(this);" tcolor="#4C85D8">성재가</span>


		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">너 그런 거 막 말하고 다녀도 괜찮은 거야?</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">아 괜찮아, 어차피 너 말고 아무도 몰라.</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">너만 조심하면 돼.</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">자세한 건 나도 잘 모르는데</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">나도 다른 사람한테 들은 거라..</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">그런 거 이야기하면 괜히</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">우리만 피곤해져 그만둬.</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">누가 그런 거로 일러바치어서</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">그 친구 맨날 교무실 불려가던데 불쌍하다</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">야 이번에 그 프로그램 다 터지고 나서 아무도 안 쓰잖아</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">너도 이참에 싹 바꿔라.</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">반성하는 게 안 보인다니까?</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">지가 잘못 될 거 같으니 태세 전환하던데 역겹다.</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">사실 저 새끼 처음부터 마음에</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">안 들어서 그냥 이유 없이 싫다.</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">넌 그걸 왜 지금 말해 중요한 건</span>
		<span style="color:#000100"onclick="dispClick(this);" tcolor="#000100">바로바로 말했어야지.</span>




		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">2007년 5월 13일 일</span>
		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">난이책을 읽고나서 우리나라가 소중한지</span>
		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">알았다 우리나라를 위해 싸워준 군</span>
		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">사나 장군께 정말 눈물이 뚝뚝 떨어지도록</span>
		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">감사해야겠다, 그중에서 이순신장군</span>
		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">은 바다에서 싸웠기 때문에 더욱</span>
		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">훌륭하다고 생각한다 이제부터 더욱</span>
		<span style="color:#735A8C"onclick="dispClick(this);" tcolor="#735A8C">공부를 열심히 해야겠다</span>



		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">저놈은 백날 해봐야 의미 없는 짓을</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">왜 해 머리가 비었구나! 비었어</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">왜 갑자기 나대?</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">평소에나 잘할 것이지.</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">그니까 어차피 열심히 해도 하는 </span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">사람들은 똑같이 한다니까?</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">내가 봤는데 술 진짜 못하더라</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">난 거짓말인 줄 알았는데</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">완전히 생긴 건 그렇게 생겼으면서.</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">말 안할게 나 입 무거워</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">나한테만 알려줘.</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">이거 진짜 비밀이다?</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">요즘 그거 때문에</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">완전 시끌시끌하잖아 몰랐어?</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">완전 범죄자네 나쁜 새끼.</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001"> 저 녀석 언젠가는 사고 한번 칠 줄 알았지.</span>
		<span style="color:#000001"onclick="dispClick(this);" tcolor="#000001">. 자기랑 똑같은 새끼 만나봐야 정신 차리지</span>

		

		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">진짜 그렇게 말했어?</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">대박 어이없다...</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">그 친구 코로나 걸려서</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">지금 격리 중이잖아.</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">나한테 옮기는 건 아니겠지?</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">아니 글쎄 오늘 그런 일이 있었다니깐?</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">너는 내 편 들어줘. 들어줄 거지?</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">결국 실패했다더라?</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">그럴 줄 알았어.</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">그 학원 학부모들이 막 찾아가고</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">난리가 나라고 그랬어.</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">망했게 망했어. 직접 가본 건 아닌데 그냥 누구한테 들었어.</span>
		<span style="color:#020000"onclick="dispClick(this);" tcolor="#020000">그 학교 질 나쁜 학교라고 소문 자자하잖아.</span>






		<span style="color:#FF7733"onclick="dispClick(this);" tcolor="#FF7733">2007년 3월 26일 월</span>
		<span style="color:#FF7733"onclick="dispClick(this);" tcolor="#FF7733">아치볼드에게</span>
		<span style="color:#FF7733"onclick="dispClick(this);" tcolor="#FF7733">아치볼드야 내가 너보다 아주 훌륭한 사</span>
		<span style="color:#FF7733"onclick="dispClick(this);" tcolor="#FF7733">람이 되면 나는 무엇이될까? 축구선수?</span>
		<span style="color:#FF7733"onclick="dispClick(this);" tcolor="#FF7733">대통령? 다른외에무엇일까? 니가</span>
		<span style="color:#FF7733"onclick="dispClick(this);" tcolor="#FF7733">하고있는탐정일까 나는 빨리 어른되고</span>
		<span style="color:#FF7733"onclick="dispClick(this);" tcolor="#FF7733">싶다 너처럼</span>



		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">2007년 3월 27 월</span>
		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">그것을 알고싶다</span>
		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">나는 이책을 읽고나서 공기가</span>
		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">업으면 소리가않난다는것을 알았다</span>
		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">그리고 공가예 힘을 얌보면 큰코를</span>
		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">타친다는걸 알았다 공기가 </span>
		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">없으면 숨을 못신다는것은 알았지만</span>
		<span style="color:#F4E131"onclick="dispClick(this);" tcolor="#F4E131">신기했다</span>


		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">2007년 4월 2일 월</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">나는 이 책을읽고 나서</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">식물에 생태을 알수있었다</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">나팔꽃은 다른 꽃이랑 다르다</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">왜냐하면 다른 꽃은 시들을까지 꽃을 피는데</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">나팔꽃은 아침에 피고</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">저녁에진다</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">난그게 신기하였다.</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">또언덴건 잎을 만지면 오모리드</span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">는 것도있다 그리고 곤충을 잡아먹는 </span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">파리지옥도 있다. 그런게알지만 </span>
		<span style="color:#B9BF04"onclick="dispClick(this);" tcolor="#B9BF04">나팔꽃을 잘몰랐다.</span>







		

		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">저들만 없었더라면 우리는 이렇게</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">내가 힘들지는 않았을 거야.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">나는 이 사화를 어지럽히는</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">당신들과 함께 살 수 없어.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">너 그 지하철 빌련 영상 봤어?</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">진짜 민폐가 따로 없지.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">당신들 때문이야 당신들 때문에 내가 이렇게 된 거라고게</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">여보세요? 야 그 소문 진짜야?</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">왜 그렇게 안 봤는데 진짜 미친 사람이었네.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">요즘 것들은 어리다고 봐주면 안 돼 아주 기어오른다니까.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">버릇을 고쳐놔야 해.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">그 소문 진짜 무섭다는 나라면</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">절대 시도도 못 했을 거야.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">그러니 벌 받았지, 어휴 꼬신다.</span>
		<span style="color:#010000"onclick="dispClick(this);" tcolor="#010000">아니 그런 사람인 줄 알았으면 나도 다른 사람이랑 어울릴걸.</span>









		</div>
	</body>
</html>
