<script>
  
</script>

<main>
  <!-- Banner Section -->
  <div class="banner relative bg-gray-900 bg-cover bg-center h-screen">
    <!-- Navbar -->
    <div class="navbar flex justify-between items-center p-4 bg-black/70 backdrop-blur-lg rounded-lg shadow-lg">
      <!-- Social Links -->
      <div class="flex space-x-6">
        {#each [
          { href: "https://www.facebook.com/dabuedison", icon: "fab fa-facebook-f" },
          { href: "https://www.tiktok.com/@riespire", icon: "fab fa-tiktok" },
          { href: "https://github.com/DabuEdison", icon: "fab fa-github" },
          { href: "https://www.instagram.com/dabuedison", icon: "fab fa-instagram" },
        ] as { href, icon }}
          <a href={href} target="_blank" class="text-white hover:text-yellow-400 transition duration-300">
            <i class={`${icon} fa-lg`}></i>
          </a>
        {/each}
      </div>

      <!-- Navigation Links -->
      <nav>
        <ul class="flex space-x-6 list-none">
          {#each [
            { href: "home", label: "Portfolio" },
            { href: "about", label: "About" },
            { href: "contacts", label: "Contact" },
          ] as { href, label }}
            <li>
              <a href={href} class="text-white hover:text-yellow-400 transition duration-300">{label}</a>
            </li>
          {/each}
        </ul>
      </nav>
    </div>

    <div class="portfolio-section flex flex-col md:flex-row items-center justify-center text-center md:text-left mt-10">
      <img src="myphoto.jpg" alt="Edison G. Dabu" class="profile-image w-60 h-60 md:w-80 md:h-80 rounded-full object-cover shadow-lg md:mr-10 transition-transform duration-300 hover:scale-105" />
      
      <div class="portfolio-text mt-6 md:mt-0">
        <h1 class="text-5xl text-white font-extrabold mt-4">I'm <span class="highlight text-yellow-400">Edison G. Dabu</span></h1>
        <p class="text-white mt-4 max-w-2xl mx-auto leading-relaxed">I am a student at Gordon College, pursuing a Bachelor of Science in Information Technology. 
          I have a strong interest in learning website design and creating user-friendly systems. 
          I enjoy solving puzzles, playing games, and participating in the sport of sepak takraw.
        </p>
      </div>
    </div>
  </div>

  <!-- Journey as a Player -->
  <div class="portfolio-text bg-gray-900 text-white py-8 mt-5 rounded-lg shadow-lg">
    <h1 class="text-5xl font-extrabold mt-4 text-center">My Journey in <span class="highlight text-yellow-400">Sepak Takraw</span></h1>
    
    <!-- Image Gallery -->
    <div class="flex flex-col md:flex-row justify-center mt-6 space-y-4 md:space-y-0 md:space-x-4">
      {#each [
        { src: "ccs.jpg", alt: "Sepak Takraw" },
        { src: "ccs2.jpg", alt: "Sepak Takraw" },
        { src: "ccs3.jpg", alt: "Sepak Takraw" },
      ] as { src, alt }}
        <img src={src} alt={alt} class="w-60 h-60 object-cover rounded-lg shadow-lg transition-transform duration-300 hover:scale-105" />
      {/each}
    </div>

    <p class="mt-4 max-w-2xl mx-auto text-center px-4 leading-relaxed text-gray-200 bg-gray-800 p-6 rounded-lg shadow-md">
      I didn’t participate in sports during elementary school until a friend invited me to join the Sepak Takraw team for our sports fest. Even though I didn’t know how to play at first, I quickly learned and found myself enjoying it. Our team won the district meet, and we advanced to the city finals, though we fell short of the championship. This experience sparked my love for Sepak Takraw.
      Throughout high school, I continued to represent my school in district meets, though we never reached the championship. Now in college, I was excited to be selected for the CCS Sepak Takraw team. Despite a tough loss in the first round and an intense fight for the championship, we secured the bronze medal after a rematch, marking a proud achievement for CCS and a memorable milestone in my Sepak Takraw journey.
    </p>
  </div>

  <!-- Journey as an IT student -->
  <div class="portfolio-text bg-gray-900 text-white py-8 mt-5 rounded-lg shadow-lg">
    <h1 class="text-5xl font-extrabold mt-4 text-center">My Journey as <span class="highlight text-yellow-400">IT Student</span></h1>
    
    <!-- Image Gallery -->
    <div class="flex flex-col md:flex-row justify-center mt-6 space-y-4 md:space-y-0 md:space-x-4">
      {#each [
        { src: "hunt.jpg", alt: "Game development" },
        { src: "ecommerce.jpg", alt: "eshop" },
        { src: "networking.jpg", alt: "design" },
      ] as { src, alt }}
        <img src={src} alt={alt} class="w-60 h-60 object-cover rounded-lg shadow-lg transition-transform duration-300 hover:scale-105" />
      {/each}
    </div>

    <p class="mt-4 max-w-2xl mx-auto text-center px-4 leading-relaxed text-gray-200 bg-gray-800 p-6 rounded-lg shadow-md">
      In the first picture, taken during my 1st year, 2nd semester, we had a group activity where we developed a game using Java. Through this experience, I learned how to effectively communicate with my group members and share knowledge. We collaborated on applying what we had learned to develop our system.
      In the second picture, we worked on a group project, as well as an individual assignment, where we implemented a system using Angular with an API. I found the system I was assigned to be particularly challenging because there were limited resources available. Many of the tutorials I watched didn’t cover working with APIs in detail, which made implementing my e-commerce project more difficult.
      In the last photo, I demonstrated my ability to connect a switch to a PC and identify its IP address. This helped me better understand network configurations and device communication.
    </p>
  </div>
</main>
