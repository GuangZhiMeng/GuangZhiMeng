## Hi there 👋 光之梦的Github
**Nice to see you.**
**Welcome to My GitHub**
---

![image](https://user-images.githubusercontent.com/84832795/212478754-bb2b6468-c2ef-486b-ae8b-a79a0faf715d.png)
<br/>

### Github提交次数
<br/>

<div align="center"> <img height="137px" src="https://github-readme-stats.vercel.app/api?username=GuangZhiMeng&show_icons=true&hide=contribs,prs&cache_seconds=86400&theme=react" /> </div>

<div align="center"> <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=GuangZhiMeng&hide_title=true&hide_border=true&layout=compact&bg_color=0,73FA79,73FDFF,D783FF&theme=graywhite&locale=cn" /></div>

<!-- Awesome repo 比较好的仓库-->
<a href="https://github.com/GuangZhiMeng/JavaStudy">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=GuangZhiMeng&repo=github-readme-stats&cache_seconds=86400&theme=shadow_blue" /></a>
<br/>
  
<!-- visitor statistics logo 访客数统计徽标 -->
<img src="https://komarev.com/ghpvc/?username=GuangZhiMeng&label=Views&color=0e75b6&style=flat" alt="访问量统计" />

<!-- 连续打卡 -->
<div align="center"> <img src="https://github-readme-streak-stats.herokuapp.com/?user=GuangZhiMeng" /> </div>

🧰 常用的工具<br/>
![Linux Badge](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=000&style=flat)
![Windows Badge](https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=fff&style=flat)
![Visual Studio Code Badge](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?logo=visualstudiocode&logoColor=fff&style=flat)
![Adobe Photoshop Badge](https://img.shields.io/badge/Adobe%20Photoshop-31A8FF?logo=adobephotoshop&logoColor=fff&style=flat)
![GitHub Badge](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=fff&style=flat)

<!-- programming tool icon 编程工具图标 -->
<img src="https://skillicons.dev/icons?i=ps,pr,c,cpp,idea,git" /><br>
<!-- svg -->

# Visit https://github.com/lowlighter/metrics#-documentation for full reference
name: Metrics
on:
  # Schedule updates (each hour)
  schedule: [{cron: "0 * * * *"}]
  # Lines below let you run workflow manually and on each commit
  workflow_dispatch:
  push: {branches: ["master", "main"]}
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          # Your GitHub token
          # The following scopes are required:
          #  - public_access (default scope)
          # The following additional scopes may be required:
          #  - read:org      (for organization related metrics)
          #  - read:user     (for user related data)
          #  - read:packages (for some packages related data)
          #  - repo          (optional, if you want to include private repositories)
          token: ${{ secrets.METRICS_TOKEN }}

          # Options
          user: GuangZhiMeng
          template: classic
          base: header, activity, community, repositories, metadata
          config_timezone: Asia/Shanghai
          plugin_isocalendar: yes
          plugin_isocalendar_duration: full-year
          plugin_languages: yes
          plugin_languages_analysis_timeout: 15
          plugin_languages_analysis_timeout_repositories: 7.5
          plugin_languages_categories: markup, programming
          plugin_languages_colors: github
          plugin_languages_limit: 8
          plugin_languages_recent_categories: markup, programming
          plugin_languages_recent_days: 14
          plugin_languages_recent_load: 300
          plugin_languages_sections: most-used
          plugin_languages_threshold: 0%

