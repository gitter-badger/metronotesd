**@adamkrellenstein:**

- Quality Assurance
- Update `CHANGELOG.md`
- Update `lib.config.py`: `VERSION_*`
- Update `protocol_changes.json` (if necessary)
- Update `setup.py`
- Update test suite (as necessary)
- Run test suite
- Update documentation (as appropriate).
- Tag and Sign Release
- Merge branch into both `master` and `develop`
- Rebase `gh-pages` to `master`
- Write [Release Notes](https://github.com/Metronotes/metronotesd/releases)
- Upload (signed) package to PyPi
	* `sudo python3 setup.py sdist build`
	<!-- * `sudo python3 setup.py bdist_wheel build`	# Does not work with `apsw` and `ethereum-serpent` installs. -->
	* `twine upload -s dist/$NEW_FILES`

**@ivanazuber:**:

- Post to [Official Forums](https://forums.metronotes.io/discussion/445/new-version-announcements-metronotes-and-metronotesd), Skype, [Gitter](https://gitter.im/Metronotes)
- Post to social media
- SMS and mailing list notifications
