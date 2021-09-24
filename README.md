# :tomato: Pomodoro Timer in Bash

A timer for managing pomodoros from terminal, with optional interfaces for `yad`, `zenity`, and `kdialog`.

# :film_strip: Screencast

[![asciicast](https://asciinema.org/a/437736.svg)](https://asciinema.org/a/437736)

# :hammer: Usage

See `Pomodoro --help` any time for reference. Reiterated here is:

* `-t, --tag` whether to supply focus tag, defaults to "Other"
* `-d, --duration` duration of focus, defaults to 25 minutes
* `-b, --break` duration of break, defaults to 5 minutes
* `-f, --file` file path of focus histories, defaults to \$XDG_DATA_HOME
* `-i, --interface` interface to use, "terminal", "yad", "zenity" or "kdialog" (default)

Use p to toggle pause, q to quit at current time, i to increase seconds and
  any other input to skip seconds.

# :vhs: Installation

Simply copy the `Pomodoro` script to your scripts folder. If you do not have one, the basic steps of setting up one is as follows:

1. Make a `Scripts` directory anywhere in your home folder, copying the script into said folder. For instance:


```bash
mkdir ~/Scripts
wget -nd -P ~/Scripts \
https://raw.githubusercontent.com/TerseTears/pomodoro-bash/main/Pomodoro
```

2. Make the script executable

```bash
chmod +x ~/Scripts/Pomodoro
```

3. Add the path to the scripts directory in your bash profile to your `PATH` variable: Edit the `.bashrc` file, e.g. `micro ~/.bashrc`, and add the following line:

```bash
export PATH=$PATH:~/Scripts
```

