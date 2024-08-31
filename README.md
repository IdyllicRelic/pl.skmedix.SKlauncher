# Unofficial flatpak of SKlauncher for minecraft
To install this flatpak, clone this repo and build it using flatpak builder

Note: It requires flatpak-builder
``` bash
  git clone https://github.com/Reizij/pl.skmedix.SKlauncher.git
  cd pl.skmedix.SKlauncher

  # If using flatpak-builder installed from your distro's repos
  flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir pl.skmedix.SKlauncher.yml

  # If using flatpak-builder installed from flathub
  flatpak run org.flatpak.Builder --force-clean --sandbox --user --install-deps-from=flathub --repo=repo builddir pl.skmedix.SKlauncher.yml
  flatpak remote-add --user --no-gpg-verify sklauncher file://$(pwd)/repo
  flatpak install --user -y sklauncher pl.skmedix.SKlauncher



