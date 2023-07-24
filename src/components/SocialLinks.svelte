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

<ul class="w-40 lg:w-8 lg:h-36 justify-between flex lg:flex-col lg:fixed bottom-10 mb-4 lg:mb-0">
  {#each SocialLinks as SocialLink}
    <li class="h-6 w-6">
      <a href={SocialLink.link} target="_blank">
        <img src={SocialLink.icon} alt={SocialLink.name}/>
      </a>
    </li>
  {/each}
</ul>
