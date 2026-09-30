# Game Programming Project Dependencies
Separate repository for the dependencies only.

## Download
```sh
git clone --recurse-submodules https://github.com/Chris-Carvelli/game-programming-project-dependencies.git
```

## Build
```sh
mkdir build
cmake . -B build -DCMAKE_BUILD_TYPE=DEBUG
```

Once you've build this repository, you can build any student project as
```sh
mkdir build
cmake . -B build -DCMAKE_PROJECT_TYPE=DEBUG -DEXTERNAL_LIBS_FOLDER_SRC=<absolute_path>/project-dependencies -DEXTERNAL_LIBS_FOLDER_BUILD=<absolute_path>/project-dependencies/build
```

If you're running from an IDE, you can set `EXTERNAL_LIBS_FOLDER_SRC` and `EXTERNAL_LIBS_FOLDER_BUILD` from the cache.