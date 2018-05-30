# Git client comparison

В качестве проекта по предмету "Эргономика человеко-машинного взаимодействия" мы сравниваем эффективность выполнения типовых заданий в разных интерфейсах системы git. Для сравнения мы выбрали терминальный интерфейс и официальный десктопный клиент от GitHub.

От вас требуется включить запись экрана и выполнить задание, описанное ниже, последовательно в двух клиентах. Запись экрана необходима для измерения времени выполнения заданий.

После завершения выполнения задания нужно отправить записанное видео одним из следующих способов:

- **Telegram**: [romikabi](https://tele.click/romikabi) или [heykarolina](https://tele.click/heykarolina)
- **VK**: https://vk.com/romikabi или https://vk.com/heykarolina
- **Почта**: abuzyarovroman@gmail.com или tretyakovakarolina@gmail.com
- Если вам важно оставаться анонимным, можно загрузить видео на какой-либо хостинг (например, на https://gofile.io)

После этого нужно ответить на два вопроса с выбором варианта ответа по поводу опыта использования клиентов в [форме](https://goo.gl/forms/HEYy907vkj1oUS8H3). Там же можно указать ссылку на загруженное видео.

### Установка клиентов

#### Desktop

Описание установки десктопного клиента GitHub можно найти [здесь](https://github.com/desktop/desktop).

#### Terminal

Описание установки терминального клиента git можно найти [здесь](https://gist.github.com/derhuerst/1b15ff4652a867391f03#file-mac-md).

### Запись экрана

#### MacOS

Открыть QuickTime Player и выбрать пункт Файл->Новая запись экрана.

#### Windows 10

Нажать сочетание клавиш Win+G, дальше понятно.

### Важно

1. Перед выполнения задания создайте папку с названием `git-compare` и перейдите в нее командой `cd path-to-git-compare`. 
2. Создавать файлы можно любым наиболее удобным для вас способом (в терминале это можно сделать с помощью команды `touch file.txt`, которая создаст файл в текущей директории).
3. В процессе выполнения задания можно гуглить, при этом не нужно останавливать запись экрана.
4. Порядок использования клиентов вам сообщён отдельно, придерживайтесь его, так как это важно для статистического исследования. Если сомневаетесь, спросите по контактам, указанным выше.
5. Задания направлены не на или проверку навыков работы с системой git, а на сравнение эффективности работы в разных клиентах. 
6. Не прерывайте выполнение задания (между клиентами можно) и не выполняйте его больше одного раза, важен первый результат.

### Задание

1. Создайте локальный репозиторий с названием `compare-git-gui`, если вы выполняете задание через клиент от GitHub, или репозиторий с названием `compare-git-terminal`, если выполняете задание через терминал.
2. Создайте файл с названием `index.txt` в этом репозитории.
3. Скопируйте в этот файл следующий текст:

```
This is my initial commit
```

4. Закоммитьте изменения с описанием коммита `Initial commit`.

5. Создайте новую ветку `feature-1` и перейдите в нее.
6. Дополните файл `index.txt` следующей строкой:

```
This is my feature commit
```

После этого он должен иметь такой вид:

```
This is my initial commit
This is my feature commit
```

7. Создайте файл `file.txt` и скопируйте в него текст:

```
This is a new file
```

8. Закоммитьте файл `index.txt` с описанием коммита `Index changes`.
9. Закоммитьте файл `file.txt` с описанием коммита `New file created`.
10. Перейдите в ветку `master` и вмержите ветку `feature-1` в `master`.
11. Добавьте в файл `index.txt` следующую строку:

```
c00L mast3r c0mmit
```

После этого он должен иметь такой вид:

```
This is my initial commit
This is my feature commit
c00L mast3r c0mmit
```

12. Закоммитьте изменения с описанием коммита `Added c0oL stuff`.
13. Перейдите в ветку `feature-1` и добавьте в файл `index.txt` следующую строку:

```
Boring feature commit.
```

После этого он должен иметь такой вид:

```
This is my initial commit
This is my feature commit
Boring feature commit.
```

14. Закоммитьте изменения с описанием коммита `Added boring stuff`.
15. Вмержите ветку `master` в ветку `feature-1` и разрешите конфликт так, чтобы файл `index.txt` выглядел следующим образом:

```
This is my initial commit
This is my feature commit
Boring feature commit.
c00L mast3r c0mmit
```

16. Закоммитьте изменения.

