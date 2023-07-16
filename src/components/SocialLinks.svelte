<script>
  const SocialLinks = [
    {
      name: "Github",
      link: "https://github.com/asarelcastellanos",
      icon: '../../socialIcons/github.svg'
    },
    {
      name: "LinkedIn",
      link: "https://www.linkedin.com/in/asarelcastellanos/",
      icon: '../../socialIcons/linkedin.svg'
    },
    {
      name: "Twitter",
      link: "https://twitter.com/asarelathome",
      icon: '../../socialIcons/twitter.svg'
    },
    {
      name: "Instagram",
      link: "https://www.instagram.com/asarelcastellanos/",
      icon: '../../socialIcons/instagram.svg'
    },
  ];
</script>

<ul class="bg-slate-200 w-60 md:w-8 md:h-52 justify-between flex md:flex-col md:fixed md:bottom-8 md:left-8">
  {#each SocialLinks as SocialLink}
    <li class="h-8 w-8">
      <a href={SocialLink.link} target="_blank">
        <img src={SocialLink.icon} alt={SocialLink.name}/>
      </a>
    </li>
  {/each}
</ul>
