## Системные требования

* Программы: Ruby, VirtualBox, Vagrant
* Железо: 64-битный процессор с поддержкой аппаратной виртуализации, 2Гб памяти

## Создание базового бокса

    git clone https://github.com/aminin/basebox.git
    cd basebox

    bundle install
    bundle exec veewee vbox build development
    bundle exec veewee vbox halt development
    bundle exec veewee vbox export development
    vagrant box add ubuntu-12.04-server-amd64 development.box
    bundle exec veewee vbox destroy development

