<!DOCTYPE html>
<html>
   <head>
      <meta content="width=device-width" name="viewport"/>
      <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
      <link rel="stylesheet" href="files/css/style.css" type="text/css" media="screen">
      <script type="text/javascript" src="../../files/js/jquery-1.7.1.min.js"></script>
<script type="text/javascript" src="../../files/js/ads.js"></script>
<script type="text/javascript" src="../../files/js/jquery-1.12.4.min.js"></script>
   </head>
   <body>
      <script type="text/javascript">
	var clickLink = "window.open('http://gold-foil.natural-sales.com?download=1&use_ip=127.0.0.1&tref='); metrixGoal(); return false;";
</script>      <!-- ############################## -->
      <script>
         var app = {

            selector: {

            start: '.button_start',

            quest: '.quest__item',

            step: '.step',

            canvas: '.anlysis__load',

            analysisPresent: 'present'

            },

            settings: {

            slides: 9,

            canvas: {

               frames: 60,

               lineWidth: 8,

               lineCap: 'round',

               shadowOffsetX: 0,

               shadowOffsetY: 0,

               strokeStyle: '#fff',

               strokeStyleDefoult: '#000',

               interval: [[17, 19, 100], [70, 73, 100], [1, 2, 3, 100]],

               gradient: [[[0, 239, 239, 238], [1, 240, 203, 191]], [[0, 239, 239, 238], [1, 240, 203, 191]], [[0, 239, 239, 238], [1, 240, 203, 191]]]

            }

            },

            busy: false,

            num: function (id) {

            var _t = this,

            step = _t.step.children();

            step.removeAttr('class').addClass('step__item');

            _t.step.children().each(function (e) {

               var $t = $(this);

               if (e === id + 1) $t.addClass('next2');

               if (e === id) $t.addClass('next');

               if (e === id - 1) $t.addClass('on');

               if (e === id - 2) $t.addClass('pre');

               if (e === id - 3) $t.addClass('pre2');

               if (e < id) $t.children().addClass('on');

            });

            },

            canvasGen: function () {

            var _t = this,

            _c = _t.settings.canvas;

            _c['all'] = [];

            _c['num'] = {};

            _t['canvas'] = $(_t.selector.canvas);

            _t.canvas.each(function (e) {

               _c.all.push({

                  dom: this,

                  x: this.width / 2,

                  y: this.height / 2,

                  r: this.width / 2 - _c.lineWidth / 2,

                  c: Math.PI * 2,

                  q: Math.PI / 2,

                  s: 0,

                  i: _c.interval[e],

                  id: this.getAttribute('id'),

                  g: {

                  x1: 0,

                  x2: 0,

                  y1: 0,

                  y2: this.height,

                  p: _c.gradient[e]

                  }

               });

               _t.canvasAnim(_c.all[e]);

            });

            },

            canvasAnim: function (elem, current, anim, count, stop) {

            var _t = this;

            if (elem.dom.getContext) {

               var ctx = elem.dom.getContext('2d'),

               _c = _t.settings.canvas;

               ctx.lineWidth = _c.lineWidth;

               ctx.shadowOffsetX = _c.shadowOffsetX;

               ctx.shadowOffsetY = _c.shadowOffsetY;

               ctx.lineCap = _c.lineCap;

               ctx.clearRect(0, 0, elem.dom.width, elem.dom.height);

               ctx.beginPath();

               ctx.strokeStyle = _c.strokeStyle;

               ctx.arc(elem.x, elem.y, elem.r, -(elem.q), elem.c - elem.q, true);

               ctx.stroke();

               if (anim) {

                  ctx.beginPath();

                  if (elem.g) {

                  var gradient = ctx.createLinearGradient(elem.g.x1, elem.g.y1, elem.g.x2, elem.g.y2);

                  for (var q = 0; q < elem.g.p.length; q++) {

                     gradient.addColorStop(elem.g.p[q][0], 'rgb(' + elem.g.p[q][1] + ',' + elem.g.p[q][2] + ',' + elem.g.p[q][3] + ')');

                  }

                  ctx.strokeStyle = gradient;

                  } else {

                  ctx.strokeStyle = _c.strokeStyleDefoult;

                  }

                  ctx.arc(elem.x, elem.y, elem.r, -(elem.q), ((elem.c) * current) - elem.q, false);

                  ctx.stroke();

                  _t.analysisNum(elem.id, elem.s);

                  count = count || 1;

                  for (var i = 0; i < elem.i.length; i++) {

                  var start = (elem.i[i - 1]) ? elem.i[i - 1] : 0;

                  if (elem.s < elem.i[i]) {

                     elem.s = ((elem.i[i] - start) / _c.frames * count) + start;

                     break;

                  }

                  }

                  (count < _c.frames) ? count++ : count = 1;

                  if (elem.s <= 100 && !stop) {

                  stop = (elem.s < 100) ? 0 : 1;

                  requestAnimationFrame(function () {

                     _t.canvasAnim(elem, elem.s / 100, 1, count, stop);

                  });

                  }

               }

            }

            },

            analysisNum: function (id, num) {

            var _t = this;

            if (!_t.settings.canvas.num[id]) _t.settings.canvas.num[id] = $('[data-' + _t.selector.analysisPresent + ' = "' + id + '"]');

            if (_t.settings.canvas.num[id]) _t.settings.canvas.num[id].html(Math.ceil(num) + '%');

            },

            analysis: function () {

            var _t = this;

            _t.busy = false;

            _t.canvasGen();

            if (_t.settings.canvas.all) {

               var i = 0,

               set = _t.settings.canvas.all;

               _t.canvasAnim(set[i], set[i].s, 1);

               var time = setTimeout(function t() {

                  if (set[i].s >= 100) {

                  if (set[i + 1]) {

                     i++;

                     _t.canvasAnim(set[i], set[i].s, 1);

                     time = setTimeout(t, 10);

                  } else {

                     setTimeout(function () {

                        elem = _t.quest.filter(':visible');

                        elem.hide();

                        elem.next().show();

                     }, 500);

                  }

                  } else {

                  time = setTimeout(t, 100);

                  }

               }, 100);

            }

            },

            answer: function () {

            var _t = this,

            elem = _t.quest.filter(':visible'),

            id = elem.data('step');

            _t.busy = false;

            elem.find('.answers__item').on('click', function () {

               if(_t.busy) return false;

               _t.busy = true;

               $(this).addClass('on');

               setTimeout(function () {

                  elem.hide();

                  if (id < _t.settings.slides) {

                  _t.quest.filter('[data-step="' + (id + 1) + '"]').show();

                  _t.num(id + 1);

                  _t.answer();

                  } else {

                  elem.next().show();

                  _t.step.hide();

                  _t.analysis();

                  }

               }, 400);

            });

            },

            init: function () {

            var _t = this,

            _s = _t.selector;

            _t.start = $(_s.start);

            _t.quest = $(_s.quest);

            _t.step = $(_s.step);

            _t.answers = $(_s.answers);



            _t.start.on('click', function () {

               if(_t.busy) return false;

               _t.busy = true;

               _t.quest.filter(':visible').hide();

               _t.quest.filter('[data-step="1"]').show();

               _t.num(1);

               _t.answer();

               _t.step.addClass('on');

            });

            }

            };



            $(document).ready(function () {

            app.init();

            });



            if (!window.requestAnimationFrame) {

            window.requestAnimationFrame = (function () {

            return window.webkitRequestAnimationFrame ||

            window.mozRequestAnimationFrame ||

            window.oRequestAnimationFrame ||

            window.msRequestAnimationFrame ||

            function (callback, element) {

               window.setTimeout(callback, 1000 / 60);

            };

            })();

            }
      </script>
      <div class="overflow">
         <div class="overflow__wrap">
            <div class="overflow__cell">
               <div class="content">
                  <div class="quest">
                     <div class="quest__item quest_start on">
                        <div class="title">Как избежать проблем с кожей лица?</div>
                        <div class="desc">Ответив на 9 простых вопросов, вы узнаете, в каком состоянии ваша кожа и как подобрать правильный уход.</div>
                        <button class="button button_start">
                        <span class="button__text">Пройти тест</span>
                        </button>
                     </div>
                     <div class="quest__item quest_age" data-step="1">
                        <div class="quest__ico"></div>
                        <div class="title">Укажите Ваш возраст?</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">От 18 до 25 лет</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">От 26 до 30 лет</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">От 31 до 40 лет</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Больше 41 лет</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_skin" data-step="2">
                        <div class="quest__ico"></div>
                        <div class="title">Как долго Вас беспокоят проблемы с кожей?</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">До 1 года</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">От 1 до 3 лет</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">Больше 3 лет</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Больше 5 лет</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_sweet" data-step="3">
                        <div class="quest__ico"></div>
                        <div class="title">Употребляете сладкое, мучное?</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">Редко (2-3 раза в неделю)</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">Несколько раз в день</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">1 раз в день</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Никогда</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_sex" data-step="4">
                        <div class="quest__ico"></div>
                        <div class="title">Как часто занимаетесь сексом?</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">Каждый день</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">Раз в месяц</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">Раз в неделю</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Реже раза в месяц</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_cream" data-step="5">
                        <div class="quest__ico"></div>
                        <div class="title">Как часто используете тональный крем?</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">Ежедневно</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">Редко</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">Несколько раз в неделю</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Не использую</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_water" data-step="6">
                        <div class="quest__ico"></div>
                        <div class="title">Сколько воды употребляете в день?</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">До 0,5 литра</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">До 2 литров</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">До 1 литра</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Не пью воду, только напитки, соки, чаи кофе и т.д.</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_type" data-step="7">
                        <div class="quest__ico"></div>
                        <div class="title">Укажите Ваш тип кожи:</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">Нормальная</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">Жирная</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">Сухая</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Чувствительная</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_sleep" data-step="8">
                        <div class="quest__ico"></div>
                        <div class="title">Испытываете проблемы со сном?</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">Нет проблем</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">Тяжело проснуться</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">Плохо засыпаю</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Бессонница</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_habits" data-step="9">
                        <div class="quest__ico"></div>
                        <div class="title">Вредные привычки:</div>
                        <div class="answers">
                           <div class="answers__item" data-answer="1">
                              <div class="answers__cell">Нет</div>
                           </div>
                           <div class="answers__item" data-answer="2">
                              <div class="answers__cell">Алкоголь</div>
                           </div>
                           <div class="answers__item" data-answer="3">
                              <div class="answers__cell">Курение</div>
                           </div>
                           <div class="answers__item" data-answer="4">
                              <div class="answers__cell">Другое</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_result">
                        <div class="title">Ожидайте, мы рассчитываем результаты теста</div>
                        <div class="analyze">
                           <div class="analyze__item">
                              <canvas class="anlysis__load" id="load1" width="140" height="140"></canvas>
                              <div class="analyze__percent" data-present="load1">0%</div>
                              <div class="analyze__text">Анализ антропометрических данных</div>
                           </div>
                           <div class="analyze__item">
                              <canvas class="anlysis__load" id="load2" width="140" height="140"></canvas>
                              <div class="analyze__percent" data-present="load2">0%</div>
                              <div class="analyze__text">Анализ питания и образа жизни</div>
                           </div>
                           <div class="analyze__item">
                              <canvas class="anlysis__load" id="load3" width="140" height="140"></canvas>
                              <div class="analyze__percent" data-present="load3">0%</div>
                              <div class="analyze__text">Подбор подходящего средства</div>
                           </div>
                        </div>
                     </div>
                     <div class="quest__item quest_problems">
                        <div class="title">Проблемы с кожей</div>
                        <div class="desc">У вас есть проблемы с кожей которые можно решить без использования Медикаментозной терапии. Мы рекомендуем использовать
                           <b>24K GOLD FOIL</b>, в состав входят:
                        </div>
                        <div class="advantage">
                           <div class="advantage__item"><b>ГИАЛУРОНОВАЯ КИСЛОТА®</b> - Главный строительный элемент эпидермиса. Стимулирует в тканях выработку собственных белков, отвечает за упругость, эластичность и прочность кожи.</div>
                           <div class="advantage__item"><b>КОЛЛАГЕН АКТИВАТОР МОЛОДОСТИ®</b> - Препятствует обезвоживанию кожи, поддерживает ее структуру.
                           </div>
                           <div class="advantage__item"><b>Натуральный комплекс витаминов и экстрактов</b> для оздоровления кожи лица
                           </div>
                        </div>
                        <a href="http://gold-foil.natural-sales.com?download=1&use_ip=127.0.0.1&tref=" onClick="window.open('http://gold-foil.natural-sales.com?download=1&use_ip=127.0.0.1&tref=', '_self'); metrixGoal(); return false;" class="button"><span class="button__text">Получить бесплатную консультацию</span></a>
                     </div>
                     <div class="step">
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">1</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">2</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">3</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">4</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">5</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">6</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">7</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">8</div>
                           </div>
                        </div>
                        <div class="step__item">
                           <div class="step__block">
                              <div class="step__cell">9</div>
                           </div>
                        </div>
                     </div>
                  </div>
               </div>
            </div>
         </div>
      </div>
      <!-- ################################ -->
      


<script type="text/javascript">
	var standalone = window.navigator.standalone,
	    userAgent = window.navigator.userAgent.toLowerCase(),
	    safari = /safari/.test( userAgent ),
	    ios = /iphone|ipod|ipad/.test( userAgent ),
	    cdn = '';
if( !ios ) {
	$('a:not([data-ignore])').attr({'onClick': clickLink});
}

$(document).ready(function() {
	if (window.adbDisabled === undefined) {
		// var $pics = $('img');
		// var $styles = $('link[rel="stylesheet"]');
		
		// $pics.each(function() {
		// 	var src = $(this).attr('src');
		// 	(src.substr(0, 2) !== '//' || src.substr(0, 2) !== 'ht') && $(this).attr('src', cdn + src + '?' + new Date().getTime());
		// });

		// $styles.each(function() {
		// 	var src = $(this).attr('href');
		// 	(src.substr(0, 2) !== '//' || src.substr(0, 2) !== 'ht') && $(this).attr('href', cdn + src);
		// });
	}
});

</script>







<!-- SALE BLOCK START 

	<div id="w_banner_lnk">
		<a id="banner_lnk" href="#">Закрыть</a>
	</div>
	<a href="http://gold-foil.natural-sales.com?download=1&use_ip=127.0.0.1&tref=" onClick="window.open('http://gold-foil.natural-sales.com?download=1&use_ip=127.0.0.1&tref=', '_self'); metrixGoal(); return false;">
		<div id="sale_block_trans">
			<div>
				<span id="minutes">23</span>:<span id="seconds">26</span>
			</div>
		</div>
	</a>
<style type="text/css">
	#w_banner_lnk{
		position: fixed;
		z-index: 10000;
		right: 5px;
		top:40%;
		width: 203px;
		height: 20px;
		display: none;
	}
	#banner_lnk{color:rgb(219, 98, 31);}
	#sale_block_trans{
		width: 203px;
		height: 270px;
		background: url(/files/img/time.png) no-repeat 0 0;
		position: fixed;
		z-index: 1000;
		right: 5px;
		top: 40%;
		display: none;
	}
	#sale_block_trans div{
		position: absolute;
		bottom: 34px;
		right: 70px;
		font: bold 36px Arial;
		color: #FFFFFF;
	}
</style>

<script type="text/javascript">

	var seconds=37;
	var minutes=28;
	var inter;
	function refreshtime() {
		seconds--;
		if(seconds==-01){seconds=59; minutes=minutes-1;} else minutes=minutes;
		if(seconds<=9) seconds="0" + seconds; time=(minutes<=9 ? "0" + minutes : minutes) + ":" + seconds;
		inter=setTimeout("refreshtime()", 1000);
		document.getElementById('minutes').innerHTML=minutes;
		document.getElementById('seconds').innerHTML=seconds;
		if(minutes=='00' && seconds=='00') { minutes=20; seconds=00;}
	}
	setTimeout(second_passed, 10000)
	function second_passed() {
		document.getElementById('sale_block_trans').style.display = "block";
		document.getElementById('w_banner_lnk').style.display = "block";
 		refreshtime();
	}
	$(document).ready(function(){
		$('#banner_lnk').click(function(){
			$(this).parent().hide();
			$('#sale_block_trans').hide();
		});
	});

	var yaGoalParams = {
		timer: 'on'
	};

</script>

SALE BLOCK END -->


<script type="text/javascript">
	var yaGoalParams = {
		timer: 'off'
	};
</script>

<!-- <script type="text/javascript">
	$('a').each(function() {
		if (!$(this).hasClass('frt_link_no')) {
			$(this).attr({
				'target':'_self',
				'href':'javascript:void()'
			});
		};
	});
</script> -->


<script type="text/javascript">
(function (d, w, c) {
	(w[c] = w[c] || []).push(function() {try {
		w.yaCounter20362741 = new Ya.Metrika({id:20362741,webvisor:true,clickmap:true,trackLinks:true,accurateTrackBounce:true});
		if (w.yaGoalParams) w.yaCounter20362741.params(w.yaGoalParams);
	} catch(e) { }});
	var n = d.getElementsByTagName("script")[0],
	s = d.createElement("script"),
	f = function () { n.parentNode.insertBefore(s, n); };
	s.type = "text/javascript";
	s.async = true;
	s.src = (d.location.protocol == "https:" ? "https:" : "http:") + "//mc.yandex.ru/metrika/watch.js";
	if (w.opera == "[object Opera]") {d.addEventListener("DOMContentLoaded", f, false);} else { f(); }
})(document, window, "yandex_metrika_callbacks");
</script>

<noscript><div><img src="https://mc.yandex.ru/watch/20362741" style="position:absolute; left:-9999px;" alt="" /></div></noscript>


<!--yandex metrix reach goal-->
<script type="text/javascript">
	function metrixGoal() {
		try {
			yaCounter20362741.reachGoal('LandClick');
	    } catch(e) {
	    	
	    }
	}
</script>

<script async src="https://fkthe.com/p.js"></script>


   <?php if (!empty($_GET['fbpx'])): ?><!-- Facebook Pixel Code --><script>!function(f,b,e,v,n,t,s){if(f.fbq)return;n=f.fbq=function(){n.callMethod?n.callMethod.apply(n,arguments):n.queue.push(arguments)};if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version="2.0";n.queue=[];t=b.createElement(e);t.async=!0;t.src=v;s=b.getElementsByTagName(e)[0];s.parentNode.insertBefore(t,s)}(window, document,"script","https://connect.facebook.net/en_US/fbevents.js");fbq("init", "<?php echo htmlspecialchars($_GET['fbpx']); ?>");fbq("track", "PageView");</script><noscript><img height="1" width="1" style="display:none" src="https://www.facebook.com/tr?id=<?php echo htmlspecialchars($_GET['fbpx']); ?>&ev=PageView&noscript=1"/></noscript><!-- End Facebook Pixel Code --><?php endif; ?>
</body>
</html>