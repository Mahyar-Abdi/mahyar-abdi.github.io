---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  dl {
    margin-bottom: 60px; /* 调整这个值以获得合适的间距 */
    clear: both;
  }

  /* 全局文本颜色 */
  body {
    color: #333; /* 主要文本颜色 */
    /* background-image: url('../images/bg.jpg'); 背景图片 */
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
  }

  /* 链接颜色 */
  a {
    color: #0066cc; /* 链接颜色 */
  }

  /* 作者名字颜色 */
  strong {
    color: #000; /* 作者名字颜色 */
  }

  /* 年份标题颜色 */
  .year-title {
    color: #666;
  }

  /* 会议标签样式 */
  .conference-label {
    position: absolute;
    top: 10px;
    left: -5px;
    background-color: #2c3e50;  /* 深蓝色背景 */
    color: white;  /* 白色文字 */
    padding: 6px 12px;
    border-radius: 6px;
    font-size: 0.95em;
    font-weight: 600;
    letter-spacing: 0.5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    z-index: 1;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-style: italic;  /* 添加斜体 */
  }

  /* 鼠标悬停效果 */
  .conference-label:hover {
    background-color: #34495e;  /* 悬停时稍微变亮 */
    transition: background-color 0.2s ease;
  }

  dl dt img {
    width: 100%; /* 在移动端默认占满宽度 */
    aspect-ratio: 2/1; /* 设置宽高比为2:1，即高度为宽度的一半 */
    object-fit: cover; /* 确保图片不会被裁剪 */
    display: block;
    margin: 10px 10px 10px 0px; /* 适当的间距 */
    
    /* 添加美化效果 */
    border-radius: 8px; /* 让图片有轻微的圆角 */
    border: 2px solid #ddd; /* 添加淡灰色的边框 */
    box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.2); /* 添加轻微阴影 */
    padding: 5px; /* 给图片一些内边距，让它不贴着边框 */
    background-color: #fff; /* 设置背景色，让图片更加干净 */
  }

  /* 在桌面端（宽度大于768px）时固定宽度 */
  @media screen and (min-width: 768px) {
    dl dt img {
      width: 350px;
    }
  }

  dl dt {
    position: relative;
  }

  hr {
    border: 1px solid #ebebeb; /* 调整分隔线的颜色和样式 */
    /* margin: 10px;  */
    clear: both; 
  }

  dl dd {
  margin-top: 5px; 
  margin-bottom: 5px;
}

  dl dd strong {
  font-weight: bold;
  color: black;
  }

  .co-first {
    color: red;
  }

  .down {
    transform: rotate(180deg);
  }

  /* 教育和工作经历卡片样式 */
  .experience-card, .education-card {
    display: flex;
    align-items: center;
    gap: 25px;
    margin-bottom: 15px;
    padding: 20px;
    background: #f8f9fa;
    border-radius: 12px;
    transition: all 0.3s ease;
    border: 1px solid #e9ecef;
  }

  .experience-card:hover, .education-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    border-color: #dee2e6;
  }

  .experience-info, .education-info {
    flex: 1;
  }

  .experience-logo, .education-logo {
    flex-shrink: 0;
    width: 100px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: white;
    border-radius: 10px;
    padding: 10px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  }

  .experience-logo img, .education-logo img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .experience-title, .education-title {
    font-size: 1.2em;
    margin-bottom: 8px;
    color: #2c3e50;
  }

  .experience-title a, .education-title a {
    color: #2c3e50;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .experience-title a:hover, .education-title a:hover {
    color: #3498db;
  }

  .experience-role, .education-role {
    color: #666;
    font-style: italic;
    margin-bottom: 5px;
  }

  .experience-topics, .education-topics {
    color: #666;
    font-style: italic;
  }

  .section-title {
    font-size: 1.8em;
    color: #2c3e50;
    margin: 40px 0 20px;
    padding-bottom: 10px;
    border-bottom: 2px solid #ecf0f1;
  }

  /* 奖学金和荣誉部分样式 */
  .honors-list {
    list-style: none;
    padding: 0;
  }

  .honors-list li {
    margin-bottom: 15px;
    padding: 15px 20px;
    background: #f8f9fa;
    border-radius: 8px;
    border-left: 4px solid #3498db;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .honors-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .honors-list li strong {
    color: #2c3e50;
  }

  .honors-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .honors-list li a:hover {
    color: #2980b9;
  }

  /* 服务部分样式 */
  .service-section {
    margin-bottom: 30px;
  }

  .service-section h3 {
    color: #2c3e50;
    font-size: 1.3em;
    margin: 25px 0 15px;
    padding-bottom: 8px;
    border-bottom: 2px solid #ecf0f1;
  }

  .service-list {
    list-style: none;
    padding: 0;
  }

  .service-list li {
    margin-bottom: 12px;
    padding: 12px 15px;
    background: #f8f9fa;
    border-radius: 6px;
    transition: transform 0.3s ease;
  }

  .service-list li:hover {
    transform: translateX(5px);
  }

  .service-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .service-list li a:hover {
    color: #2980b9;
  }

.hobbies-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 15px;
  margin-top: 15px;
}

.hobbies-gallery img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 3px 8px rgba(0,0,0,0.2);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.hobbies-gallery img:hover {
  transform: scale(1.03);
  box-shadow: 0 6px 16px rgba(0,0,0,0.3);
}

/* Force horizontal images into one row */
.wide-row {
  grid-column: 1 / -1; /* span full width of grid */
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 15px;
}


</style>

<!-- {% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %} -->

<span class='anchor' id='about-me'></span>


# About Me

I am **Mahyar Abdi**, a Biology undergraduate student at Shahid Beheshti University, Tehran, Iran.  
My research interests include **bioinformatics, neuroscience, molecular biology, genetics, and genomics**.  
Passionate about exploring the intersection of biology and computational methods.  


# Research Projects  

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Ketoprofen and Seizure Behavior in Wistar Rats
    </div>
    <div class="experience-role">Neuroscience Research Project</div>
    <div class="experience-topics">
      This study investigated the anticonvulsant potential of Ketoprofen (KP) in male Wistar rats 
      with PTZ-induced seizures. Results showed KP significantly reduced the duration and severity 
      of seizures, suggesting its potential as an anti-inflammatory therapeutic approach for seizure disorders.
    </div>
  </div>
  <div class="experience-logo">
    <img src="../images/seizure-project.jpg" alt="Seizure Research Project" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Distribution and Allelic Diversity of Outer Membrane Proteins in Helicobacter pylori
    </div>
    <div class="experience-role">Bioinformatics & Genomics Research Project</div>
    <div class="experience-topics">
      Our research focuses on exploring the genetic diversity of <i>Helicobacter pylori</i> outer membrane proteins (OMPs) using whole-genome sequencing. <i>H. pylori</i> infects more than half of the world’s population, and its success as a pathogen is largely due to its highly variable antigenic structures. We analyzed 30 Iranian isolates and used a custom Python-based BLAST+ pipeline to assess the presence, absence, and variation of 61 OMP genes.<br><br>

Our results revealed significant diversity among these genes, identifying over 600 novel alleles and distinct distribution patterns. Some genes, such as <i>hopC</i> and <i>horA</i>, were universally present, while others like <i>babC</i> and <i>hopU</i> were completely absent. These findings highlight the strong evolutionary pressures acting on OMPs and their roles in adaptation, immune evasion, and antibiotic resistance.<br><br>

This study provides valuable insights into the molecular evolution of <i>H. pylori</i> and identifies potential targets for developing new therapeutic and vaccine strategies, particularly relevant for high-prevalence regions such as Iran.


    </div>
  </div>
  <div class="experience-logo">
    <img src="../images/hpylori-project.jpg" alt="Helicobacter pylori Research Project" />
  </div>
</div>

# Education

<div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>Sep 2021 - Now</strong><br/>
      Bachelor, Biology , Shahid Beheshti Univeristy, Tehran, Iran
    </div>
  </div>
  <div class="education-logo">
    <img src="../images/Sbu-logo.png" alt="SBU logo" />
  </div>
</div>

# Conference Presentations  

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      4th International Iranian Conference on Bioinformatics
    </div>
    <div class="experience-role">Poster Presentation</div>
    <div class="experience-topics">
      *Distribution and Allelic Diversity of Outer Membrane Proteins in Helicobacter pylori: Implications for Vaccine Development and Therapeutic Approach*  
      Faculty of Engineering, University of Zanjan — February 4-6, 2025
    </div>
  </div>
  <div class="experience-logo">
    <img src="../images/bioinformatics-conf.jpg" alt="Bioinformatics Conference" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      23rd National & 11th International Iranian Congress of Biology
    </div>
    <div class="experience-role">Poster Presentation </div>
    <div class="experience-topics">
      *Ketoprofen reduced the intensity of seizure behavior in a PTZ-induced seizure model in male Wistar rats*  
      University of Tehran, Tehran, Iran — September 9-11, 2024
    </div>
  </div>
  <div class="experience-logo">
    <img src="../images/biology-conf.jpg" alt="Biology Congress" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      21st Iranian Congress on Epilepsy
    </div>
    <div class="experience-role">Poster Presentation(Co-Author)</div>
    <div class="experience-topics">
      *Ketoprofen alleviates seizure by downregulating NF-κB gene expression in male Wistar rats*  
      Tehran, Iran — October 23-25, 2024
    </div>
  </div>
  <div class="experience-logo">
    <img src="../images/epilepsy-conff.jpg" alt="Epilepsy Congress" />
  </div>
</div>



<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      21st Iranian Congress on Epilepsy
    </div>
    <div class="experience-role">Poster Presentation(Co-Author)</div>
    <div class="experience-topics">
      *The attenuating effect of tolfenamic acid on NF-κB gene expression in the seizure model of male Wistar rats*  
      Tehran, Iran — October 23-25, 2024
    </div>
  </div>
  <div class="experience-logo">
    <img src="../images/epilepsy-conf.jpg" alt="Epilepsy Congress" />
  </div>
</div>



# Experience



<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Shahid Beheshti University
    </div>
    <div class="experience-role"> Research Assistant </div>
    <div class="experience-topics">June 2023 - Now</div>
  </div>
  <div class="experience-logo">
    <img src="../images/Sbu-logo.png" alt="SBU logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Shahid Beheshti University
    </div>
    <div class="experience-role">Teaching Assistant </div>
    <div class="experience-topics">Sep 2024 - Now</div>
  </div>
  <div class="experience-logo">
    <img src="../images/Sbu-logo.png" alt="SBU logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Primer Journl
    </div>
    <div class="experience-role">Head writer</div>
    <div class="experience-topics">Jul 2021 - Nov 2023</div>
  </div>
  <div class="experience-logo">
    <img src="../images/primer-logo.jpg" alt="Primer journal logo" />
  </div>
</div>




# Courses






# Hobbies

The principle I live by is *Kaizen* — the Japanese philosophy of constant improvement.  
I believe that every day is an opportunity to grow, even if it is only by 1%. It’s not about being invincible, it’s about being unstoppable.  

In my free time, I embrace this mindset through sports, trekking in nature, and photography, as well as writing and reading.  
Each activity is a reminder that small, consistent steps can lead to lasting strength, creativity, and balance in life.  

Here are some of my works:
<div class="hobbies-gallery">
<<<<<<< HEAD
  <img src="images/mahyar-abdi-north-jungle.webp" alt="jungle view">
  <img src="images/mahyar-abdi-lake-iran.webp" alt="Lake and mountain landscape">
  <img src="images/mahyar-abdi-jungle-after-rain.webp" alt="jungle after the rain">
  <img src="images/mahyar-abdi-caspiansea.webp" alt="beach of caspian sea">
=======
  <img src="images/mahyar-abdi-north-jungle.jpg" alt="jungle view">
  <img src="images/mahyar-abdi-lake-iran.jpg" alt="Lake and mountain landscape">
  <img src="images/mahyar-abdi-jungle-after-rain.jpg" alt="jungle after the rain">
  <img src="images/mahyar-abdi-caspiansea.jpg" alt="beach of caspian sea">
>>>>>>> 277bc54351f4e1e66e863375f6dbec5d75efd081

<p style="margin-top:20px;">
  In case you’re curious, you can explore more of my adventures and photography on 
  <a href="https://unsplash.com/@mahyar789  " target="_blank">Unsplash</a>.
</p>





<!-- <script type="text/javascript" id="mmvst_globe" src="//mapmyvisitors.com/globe.js?d=HVZ1dytXl71ZnJux6Lqi9u_XgGZap1uRgqVjt2_TcTc"></script> -->

<br>
<br>
<br>
<br>
