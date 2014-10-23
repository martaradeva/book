# Ruby on Rails notes

**Езици за програмиране:**

*   Ruby (Руби) е език за програмиране (други: C#, Java, C++, PHP, JavaScript, Clojure, Scheme и още 2783...)
*   Код = последователност от команди и данни
*   Кодът на Ruby се пази в текстови файлове с произволен размер и брой
*   Изпълнява се от програма (интерпретатор), кръстена “ruby”
*   Може да се изпълняват и една по една, а вие да виждате резултата
*   Interactive Ruby — irb и TryRuby.org
*   Променливи и стойности
*   Типове стойности – числа, низове, списъци, речници…
*   Абстракции – методи, класове

*   Пример за ruby code:

*   5.пъти {
*   покажи_текст_на_екрана "Здравейте!"
*   }

**ОСНОВИ НА ПРОГРАМИРАНЕТО: **

*   **Данни и имена:**

*    
*   **Действия:**

**   **Условия**

*   Пример;

*   if човекът_е_гладен?
*     прати_човека_да_обядва
*   else
*     помоли_човека_да_изиграе_едно_хоро
*   end

*    
*   **Цикли**

*   *Do и end = { }

*   Примери:

*   30.times do
*        направи_коремна_преса
*   end

*

*   100.times do
*       |номер_на_участник| имейл_адрес=  
*       намери_имейла_на_участник_по(номер_на_участник)
*       изпрати_подсещащ_имейл_до(имейл_адрес)
*   end

*

*   5.пъти {
*   покажи_текст_на_екрана "Здравейте!"
*   } 

**   **Речник:**

*   **Типове уеб сайтове:**

*   **UX (user experience) = UI (user interface) + Workflow**

*   Компоненти на едно уеб приложение (бази данни, инфраструктурни компоненти)
*   Инструменти — конзола, текстов редактор, браузър
*   Rails генератори; Scaffolds; Gems и управлението им
*   MVC, REST/Resources
*   Модели и Active Record
*   Контролери и ActionController
*   Изгледи и ERB
*   Бази от данни 

**What is what? (Bento Box)**

**#1 PHP** – Logic: PHP is a very popular language designed to produce dynamic Web pages. It goes well with HTML.

**#2 SaaS** – “Software wanna be”: Software as a service. Not a technical term - more a business/delivery model, in which software is hosted centrally, not by the user themselves and they often pay a subscription fee. Examples range from Salesforce, Spotify, Google Docs.

**#3 RoR** – Logic: Ruby on Rails. Sometimes abbreviations might fool you!

**#4 HTML** - Style & structure: Especially structue: HTML is what describes the structure and the (static) content of the website. (XHTML? HTML5?)/ Scripting language vs. markup?

**#5 MongoDB** – Database: An open source database system. Stores the web app data in a little different way than MySQL, making it easier and faster for certain types of apps. What are noSQLs?

**#6 Apache** – Infrastructure: A popular open source HTTP server software. Servers can be hardware or software - here we’re focusing on the latter. Servers are the piece of software that delivers the web page to you. What is HTTP? What is the role of the browser?

**#7 CSS** - Style and structure. Especially style, designed to describe the look of webpages, including elements such as the layout, colors and fonts. Why is CSS important when building bigger sites?/What is CSS3?

**#8 Django** – Logic: A similar framework as Rails is for Ruby, Django is for Python.

**#9 MySQL** – Database: World’s most popular open source database system, used by Facebook, Twitter, Wordpress etc. Well baked into many software stacks like LAMP (open source)

**#10 nginx** – Infrastructure: Pronounced “Engine X”. An open source HTTP server. Said to be faster than Apache - in many ways like MongoDB is for MySQL./ What are proxies?

**Употреби на квадратни скоби: `[ ]`**

1.  За създаване на списък

*   dishes = ["salad", "fried chicken", "vegetable soup"]

1.  За избор на елемент от списък по негов пореден номер, например: 

*   dishes[1] # => "fried chicken"

3. За избор на стойност по ключ от речник

*   courses = {
*       appetizer: "green salad",
*       main: "fried chicken",
*       dessert: "chocolate cheese cake with mascarpone",
*   }
*   choices[:dessert] # => "chocolate cheese cake with mascarpone"