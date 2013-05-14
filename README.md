    if [ -f .zshenv ]; then cp .zshenv{,.`date +"%Y%m%d%H%M%S"`}; fi && if [ -f .zshrc ]; then cp .zshrc{,.`date +"%Y%m%d%H%M%S"`}; fi && git clone https://github.com/toshiaki61/dotfiles.git .files && echo 'source ~/.files/zsh/zshenv' > ~/.zshenv && echo 'source ~/.files/zsh/zshrc' > ~/.zshrc

    sudo chsh -s /bin/zsh `whoami`
