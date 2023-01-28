<script>
  import { onMount } from "svelte";

  let currentSiteUrl;

  onMount(()=> {
    currentSiteUrl = window.location.href;
  })
</script>

<header class="w-full fixed bottom-0 left-0 z-100 bg-stone-50 dark:bg-slate-900" id="header">
  <nav class="max-w-60.5 h-12 flex justify-between items-center mx-4 sm:mx-6 md:mx-auto">
      <a href={currentSiteUrl} class="text-zinc-800 dark:text-zinc-50">Addison</a>
      <div class="nav__menu pt-8 px-6 pb-16 fixed sm:-bottom-full left-0 w-full ra md:ml-auto" id="nav-menu">
          <ul class="nav__list grid">
              <li class="nav__item">
                  <a href="#home" class="nav__link active-link">
                      <i class="uil uil-estate nav__icon"></i> 主页
                  </a>
              </li>
              <li class="nav__item">
                  <a href="#about" class="nav__link">
                      <i class="uil uil-user nav__icon"></i> 关于
                  </a>
              </li>
              <li class="nav__item">
                  <a href="#skills" class="nav__link">
                      <i class="uil uil-file-info-alt nav__icon"></i> 技能
                  </a>
              </li>
              <li class="nav__item">
                  <a href="#services" class="nav__link">
                      <i class="uil uil-briefcase-alt nav__icon"></i> 服务

                  </a>
              </li>
              <li class="nav__item">
                  <a href="#portfolio" class="nav__link">
                      <i class="uil uil-scenery nav__icon"></i> 项目

                  </a>
              </li>
              <li class="nav__item">
                  <a href="#contact" class="nav__link">
                      <i class="uil uil-message nav__icon"></i> 联系我
                  </a>
              </li>
          </ul>
          <i class="uil uil-times nav__close" id="nav-close"></i>
      </div>

      <div class="nav__btns">
          <!-- Theme change button  -->
          <i class="uil uil-moon change-theme" id="theme-button"></i>

          <div class="nav__toggle" id="nav-toggle">
              <i class="uil uil-apps"></i>
          </div>
      </div>
  </nav>
</header>