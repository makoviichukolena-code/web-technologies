***Keepsake*** — адаптивний лендінг



Односторінковий лендінг дизайн-агенції Keepsake за макетом у Figma.

Лабораторна робота №7 (Flexbox + media-запити).



*Демо*: https://<your-username>.github.io/landing-keepsake/



***Технології***



\- HTML5 (семантична розмітка: `header`, `nav`, `main`, `section`, `article`, `footer`, `form`)

\- CSS3: Flexbox, CSS Grid, CSS-змінні, media-запити

\- Google Fonts: Oswald, Open Sans, Dancing Script (`font-display: swap`)

\- Інлайн-SVG іконки (SVG-спрайт + `<use>`)

\- Без JavaScript, фреймворків та UI-бібліотек



***Ключові рішення***



* *Mobile first*. Базові стилі для 375px, далі `@media (min-width: 768px)` і `@media (min-width: 1280px)`.
* *Дизайн-токени*. Кольори, шрифти, відступи та розміри оголошені в `:root`; на брейкпоінтах змінюються лише значення змінних.
* *Контейнер*. `width: min(100% - 2 \* var(--gutter), 1100px)`: контент центрується, горизонтального скролу немає на 320–1920px.
* *Мобільне меню без JS*. Прихований `input\[type="checkbox"]` + `label`-бургер, стан `:checked` відкриває меню, бургер перетворюється на хрестик.
* *Фільтр портфоліо без JS*. Радіокнопки + селектор `:checked \~` і атрибут `data-category`.
* *Ховер картки.* Оверлей показується на `:hover`, `:focus-visible` та `:focus-within`.
* *Форма підписки.* HTML-валідація (`type="email"`, `required`), стан помилки через `:user-invalid`, стан success через `:target` і `:has()`.
* *Fixed header* і кнопка «вгору» 44×44.
* *Доступність*. Видимий фокус, `aria-label` на іконочних кнопках, `<label>` для полів, `aria-describedby` для помилки.
* *Продуктивність*. Зображення у WebP з `width`/`height` і `loading="lazy"`.



***Структура***



```

landing-keepsake/

├── index.html

├── css/

│   ├── reset.css

│   └── style.css

├── images/

└── fonts/

```



***Запуск***



Відкрити `index.html` у браузері або запустити Live Server у WebStorm.

