<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to HomePage">Имя Фамилия</a>
        <div class="nav-links">
           {#each nav as link}
            <a href={link.href} class="link">{link.title}</a>
            {/each}
             <!--{#if link.isShow}
            <a href={link.href} class="link">{link.title}</a>
            {/if}-->
        </div>
    </div>
</nav>

<div class="container">
    <!--страницы укажем ниже-->
    <slot></slot>
</div>

<script>
    const nav = [
        {
            title: 'Обо мне',
            href: '/about',
            isShow: true,
        },
        {
            title: 'Блог',
            href: '/blog',
            isShow: true,
        },
        {
            title: 'Портфолио',
            href: '/project',
            isShow: true,
        },
        {
            title: 'Контакты',
            href: '/contact',
            isShow: true,
        },
        {
            title: 'temp',
            href: '/temp',
            isShow: false,
        },
    ]
</script>

<style>
    .container {
        max-width: 1400px;
        margin: 50 px auto;
    }
</style>