# jekyll-folder-example

Jekyll example where we use a separate branch `gh-pages` for hosting the website.

# Steps

1. Create empty branch
   ```shell
   git checkout --orphan gh-pages
   git reset --hard
   git commit --allow-empty -m "adding empty gh-pages branch"
   git push origin gh-pages
   ```

2. Generate Jekyll site
   ```shell
   jekyll new --skip-bundle .
   ```
3. Add dependencies to Gemfile
4. Install dependencies
   ```shell
   bundle install
   ```
5. Config Jekyll site `_config.yml` and `_config.development.yml`

6. Run
   ```shell
   jekyll serve --config _config.yml,_config.development.yml
   ```
7. Use Collections
