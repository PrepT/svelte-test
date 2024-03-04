<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to HomePage">Имя Фамилия</a>
        <div class="nav-links">
            <a href="/about" class="link">Обо мне</a>
            <a href="/blog" class="link">Блог</a>
            <a href="/project" class="link">Портфолио</a>
            <a href="/contact" class="link">Контакты</a>
        </div>
    </div>
</nav>

<div class="container">
    <!--страницы укажем ниже-->
    <slot></slot>
</div>

<style>
    .container {
        max-width: 1400px;
        margin: 50 px auto;
    }
</style>