# HOW TO DEPLOY?

## 1. Clone the blog repository.
git clone https://github.com/princessyv/blog.git princessyv

## 2. Initialize a new hexo template.
hexo init temp

## 3. Copy template files.
rm temp/_config.yml

cp -R temp/* princessyv/

## 4. Download newest tranquilpeak.
 https://github.com/LouisBarranqueiro/hexo-theme-tranquilpeak

## 5. Copy tranquilpeak into themes folder
cp -R tranquilpeak princessyv/themes

## 6. Copy configuration files into the theme folder.
cp princessyv/configure/_config.yml princessyv/themes/tranquilpeak/

cp princessyv/configure/zh-cn.yml princessyv/themes/tranquilpeak/languages/

cp princessyv/configure/footer.ejs princessyv/themes/tranquilpeak/layout/_partial/

## 7. Pull website from github.
cd princessyv

git clone https://github.com/princessyv/princessyv.github.io.git public

## 8. Deploy the website.
rm source/_posts/README.md

hexo g

hexo s