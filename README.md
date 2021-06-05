# ForLazyPeople
Lazy People can download a built chiapos with improvements from pechy

Built Using Instructions from TripleM99 on reddit https://www.reddit.com/user/TripleM999/
https://www.reddit.com/r/chia/comments/ns3qf0/has_someone_compiled_the_20_improvement_combined/h0kllf3?utm_source=share&utm_medium=web2x&context=3

It is not that complicated. You will need:

- Microsoft C++ Build Tools (https://visualstudio.microsoft.com/visual-cpp-build-tools/)

- Python 3.7.X

- Git

then open the x64 Native Tools Comand Prompt and input there:

cd <Wherever\you\want>

git clone https://github.com/pechy/chiapos.git

cd chiapos

git checkout 369c9e773d9d43b00696771aad46cc5b4c54e785

mkdir build && cd build

cmake ../

cmake --build . --config Release

copy Release\chiapos.cp37-win_amd64.pyd %USERPROFILE%\AppData\Local\chia-blockchain\app-1.1.6\resources\app.asar.unpacked\daemon

Edit: added --config Release to build command

Edit2: added link to Standalone MSVC Build Tools

Edit3: changed copy source
