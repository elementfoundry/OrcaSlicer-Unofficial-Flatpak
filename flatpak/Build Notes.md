Run the following commands from the terminal to build and install the flatpak. Currently this is only working with the 2.30 dev codebase.

```
flatpak-builder --ccache --force-clean --default-branch=main --install-deps-from=flathub builddir com.elementfoundry.OrcaSlicer.yml --repo=_repo

flatpak build-bundle -vv --ostree-verbose _repo Unofficial-OrcaSlicer.flatpak com.elementfoundry.OrcaSlicer --runtime-repo=https://flathub.org/repo/flathub.flatpakrepo main


```