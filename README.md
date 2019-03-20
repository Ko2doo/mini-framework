# Сборка для быстрого старта
Набор готовых правил для маленьких (и не очень) проектов без использования bootstrap'a но с использованием некоторых плюшек от туда=).

# Небольшое вступление...
Мне не очень удобен boostrap поэтому я решил сделать свою базу для быстрого старта с использованием Sass (Scss).

# Специальные классы:

* content-container

.content-container что то вроде обычного .container'a в bootstrap, работает так же =)

Пишете разметку в HTML и где нужно запихать в контейнер какой либо контент оберните его (контент) в класс .content-container.

.content-container имеет максимальную ширину: 1170px (думаю этого достаточно) конечно это можно переопределить в зависимости от вашего макета.

* card

Помните классы: col-md-6 и т.д? так вот классы: .card, .card-big, .card-mini это что то вроде того) но со свими значениями)

Например класс .card это дефолт он иметт ширину 30%

Класс .card-big 40%

Класс .card-mini 20%

* Правила записи:

Если вам нужна карточка (чего угодно не важна!) то вы можете использовать уже готовую конструкцию приведенную ниже:


<code>
	<div class="card">

		<div class="card-header">
			<!-- голова карточки -->
		</div>

		<div class="card-body">
			<!-- тело карточки -->
		</div>

	</div>
</code>


так же есть класс .shadow если вы припишете его к карточке то она будет иметь тень, по деволту она не имеет ни каких закруглений, она полностью прозрачна.


# Типография

Я использовал два шрифта на мой взгляд самые красивые (как бонус поддерживают кириллицу) это: Comfortaa и MontserratAlternates скачаны с google-fonts.

* Comfortaa
Используется как основной.

* MontserratAlternates
Используется только для заголовков всех пяти уровней


# Кнопки

Все кнопки прозрачны кроме второй (фиолетовая), есть три готовых кнопки это:

* button-default (max-width 185px)

* button-modern (max-width 185px)

* button-small (width auto)

# Для чего custom-stylesheet.scss?

В этом файле вы можете эксперементировать, переопределять стили. При использовании "штуки" можете удалить этот файл, он вам не нужен

# Маркеровка текста

Добавлено 3 класса для маркировки текста:

* text-mark-black

* text-mark-white

* text-mark-violet

# Заголовки и подзаколовки

Да да они у меня есть ниже приведу названия классов и что внутри:

* headline-big (оборачивает h1 по умолчанию 32px)

* headline-mini (оборачивает h2 по умолчанию 24px)

* headline (оборачивает h3 по умолчанию 18px)

Записываем следующим образом
<code>

	<div class="headline-big">
		<h1><!-- ваш текст --></h1>
	</div>

	<div class="headline-mini">
		<h2><!-- ваш текст --></h2>
	</div>

	<div class="headline">
		<h3><!-- ваш текст --></h3>
	</div>
</code>
