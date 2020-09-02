#https://jekyllrb.com/docs/installation/ubuntu/

sudo apt-get install ruby-full build-essential zlib1g-dev

echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

gem install jekyll bundler

#https://jekyllrb.com/docs/step-by-step/01-setup/

bundle init

bundle exec jekyll build
bundle exec jekyll serve
