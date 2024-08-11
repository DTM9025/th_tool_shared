## How to roughly compile this on Visual Studio 2017

* Make sure to consistently set the same *C/C++ → Code Generation → Runtime
  Library* option you also want to use for the main program.

* Point the compiler to the subdirectories of all dependencies by adding the
  following to the list at *C/C++ → General → Additional Include Directories*,
  **in this order**:

  ```
  $(ProjectDir)..\
  $(ProjectDir)..\bgmlib\libs\fox\include\
  $(ProjectDir)..\bgmlib\libs\ogg\include\
  $(ProjectDir)..\bgmlib\libs\vorbis\include\
  ```

## License

th_tool_shared is licensed under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

See [Touhou Music Room's `LICENSE.md`](https://github.com/DTM9025/musicroom/blob/master/LICENSE.md) for the full terms.
