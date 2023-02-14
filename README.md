# ubuntu_desktop_slideshow

copy imgchanger to /<user>/.local/bin
add to path ("export PATH=$PATH:$HOME/.local/bin")
add the following lines to end of "$HOME/.bashrc" script:
	haslocal=$(echo "$PATH" | grep "/.local")
	if [ -z "$haslocal" ]; then
		export PATH="$PATH:$HOME/.local/bin"
	fi
add to .bash_aliases ("alias imgchanger = \"imgchanger& disown\"")
add to startup (Ubuntu menu >> startup applications >> add new)
Done!

