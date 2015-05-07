OmniRom Translator Repositories
==========================

The local manifest file needed for OmniRom's translators.

These local_manifest file are dedicated for branch android-4.4
------

You need to be in your source folder.

Add TranslationTools repository:
------

If you want to add TranslationTools to help you to find untranslated strings.

    curl https://raw.githubusercontent.com/DelphinPETER/OmniRom_TranslatorRepo/android-4.4/TranslationTools.xml > .repo/local_manifests/TranslationTools.xml
    repo sync
    
When the sync is finished, you can find TranslationTools under SOURCE_FOLDER/tools/TranslationTools/binary


Add extra packages repositories:
------

If you want to get all the available OmniRom translatable packages that are not synced by default (not included in the default manifest), execute:

    curl https://raw.githubusercontent.com/DelphinPETER/OmniRom_TranslatorRepo/android-4.4/extra_packages.xml > .repo/local_manifests/extra_packages.xml
    repo sync

Hint: if you are already downloaded some device repositories with "breakfast" and have problems syncing, execute:

    rm .repo/local_manifests/roomservice.xml
    repo sync
    breakfast <device>

# OmniRom_TranslatorRepo
