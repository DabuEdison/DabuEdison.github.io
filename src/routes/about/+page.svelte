<script>
  // You can add any JavaScript logic here if needed
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
              { href: "home", label: "Home" },
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
    
    <!-- Second Portfolio Text Section -->
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
        When I was an elementary student, I didn't participate in any sports until one of my friends invited me to join the Sepak Takraw team for our sports fest. At that time, I didn’t even know how to play the game. He took the time to introduce me to the rules and flow of the game. 
        On the day of the sports fest, I was unsure if I could play. However, when I participated, I discovered that I actually enjoyed it. Our team won that day, and I was selected as a player to represent our school. This was the first time I realized how much I liked Sepak Takraw. We won our district meet, which qualified us for the city meet. During the city meet, we reached the finals, and if we had won, we would have moved on to what they called "CLARAA." Unfortunately, we lost that championship, and while they selected a player to continue, I was not chosen. 
        As I grew older, I continued to play Sepak Takraw during high school and represented my school in the district meet. Sadly, we were unable to make it to the championship during my high school years. 
        Now that I am in college, I tried out for the Sepak Takraw team and was thrilled to be selected as a player representing the CCS department. When the game day arrived, we faced the CHTM department in the first round but we lost, with a final score of 2-0 in the final set. For the championship, we had an intense match against the CEAS department, ending with a score of 2-1 in their favor. Finally, we fought for the bronze medal against the CHTM department once again, and this time we won, securing the bronze for CCS!
      </p>
    </div>
  </main>
  
  