# Dlib compiled binary wheels for Python 3.7 - 3.12 on Windows 10 X64

This repository contains the compiled binary (.whl) files for the [Dlib](http://dlib.net/) library to install on Python versions 3.7, 3.8, 3.9, 3.10, 3.11, and 3.12 on a Windows x64 OS. 

- 参考问题：https://stackoverflow.com/questions/76629574/error-could-not-build-wheels-for-dlib-which-is-required-to-install-pyproject/78611105#78611105

'''
- 错误提示；
'''
```
× Building wheel for dlib (pyproject.toml) did not run successfully.
  │ exit code: 1
  ╰─> [78 lines of output]
      running bdist_wheel
      running build
      running build_ext
      <string>:125: DeprecationWarning: distutils Version classes are deprecated. Use packaging.version instead.
      Building extension for Python 3.11.4 (tags/v3.11.4:d2340ef, Jun  7 2023, 05:45:37) [MSC v.1934 64 bit (AMD64)]
      Invoking CMake setup: 'cmake C:\Users\Jack\AppData\Local\Temp\pip-install-tl9fdcf0\dlib_fee2183dfbb9404395bfedaca5728c1a\tools\python -DCMAKE_LIBRARY_OUTPUT_DIRECTORY=C:\Users\Jack\AppData\Local\Temp\pip-install-tl9fdcf0\dlib_fee2183dfbb9404395bfedaca5728c1a\build\lib.win-amd64-cpython-311 -DPYTHON_EXECUTABLE=C:\Users\Jack\AppData\Local\Programs\Python\Python311\python.exe -DCMAKE_LIBRARY_OUTPUT_DIRECTORY_RELEASE=C:\Users\Jack\AppData\Local\Temp\pip-install-tl9fdcf0\dlib_fee2183dfbb9404395bfedaca5728c1a\build\lib.win-amd64-cpython-311 -A x64'
      -- Building for: NMake Makefiles
      CMake Error at CMakeLists.txt:5 (message):
     !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

        You must use Visual Studio to build a python extension on windows.  If you
        are getting this error it means you have not installed Visual C++.  Note
        that there are many flavors of Visual Studio, like Visual Studio for C#
        development.  You need to install Visual Studio for C++.

        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

      -- Configuring incomplete, errors occurred!
      Traceback (most recent call last):
        File "C:\Users\Jack\AppData\Local\Programs\Python\Python311\Lib\site-packages\pip\_vendor\pyproject_hooks\_in_process\_in_process.py", line 353, in <module>
          main()
        File "C:\Users\Jack\AppData\Local\Programs\Python\Python311\Lib\site-packages\pip\_vendor\pyproject_hooks\_in_process\_in_process.py", line 335, in main
          json_out['return_val'] = hook(**hook_input['kwargs'])
                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
        File "C:\Users\Jack\AppData\Local\Programs\Python\Python311\Lib\site-packages\pip\_vendor\pyproject_hooks\_in_process\_in_process.py", line 251, in build_wheel
          return _build_backend().build_wheel(wheel_directory, config_settings,
                 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\build_meta.py", line 416, in build_wheel
          return self._build_with_temp_dir(['bdist_wheel'], '.whl',
                 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\build_meta.py", line 401, in _build_with_temp_dir
          self.run_setup()
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\build_meta.py", line 338, in run_setup
          exec(code, locals())
        File "<string>", line 218, in <module>
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\__init__.py", line 107, in setup
          return distutils.core.setup(**attrs)
                 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\core.py", line 185, in setup
          return run_commands(dist)
                 ^^^^^^^^^^^^^^^^^^
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\core.py", line 201, in run_commands
          dist.run_commands()
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\dist.py", line 969, in run_commands
          self.run_command(cmd)
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\dist.py", line 1234, in run_command
          super().run_command(command)
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\dist.py", line 988, in run_command
          cmd_obj.run()
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\wheel\bdist_wheel.py", line 343, in run
          self.run_command("build")
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\cmd.py", line 318, in run_command
          self.distribution.run_command(command)
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\dist.py", line 1234, in run_command
          super().run_command(command)
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\dist.py", line 988, in run_command
          cmd_obj.run()
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\command\build.py", line 131, in run
          self.run_command(cmd_name)
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\cmd.py", line 318, in run_command
          self.distribution.run_command(command)
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\dist.py", line 1234, in run_command
          super().run_command(command)
        File "C:\Users\Jack\AppData\Local\Temp\pip-build-env-ar6t1xkr\overlay\Lib\site-packages\setuptools\_distutils\dist.py", line 988, in run_command
          cmd_obj.run()
        File "<string>", line 130, in run
        File "<string>", line 167, in build_extension
        File "C:\Users\Jack\AppData\Local\Programs\Python\Python311\Lib\subprocess.py", line 413, in check_call
          raise CalledProcessError(retcode, cmd)
      subprocess.CalledProcessError: Command '['cmake', 'C:\\Users\\Jack\\AppData\\Local\\Temp\\pip-install-tl9fdcf0\\dlib_fee2183dfbb9404395bfedaca5728c1a\\tools\\python', '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=C:\\Users\\Jack\\AppData\\Local\\Temp\\pip-install-tl9fdcf0\\dlib_fee2183dfbb9404395bfedaca5728c1a\\build\\lib.win-amd64-cpython-311', '-DPYTHON_EXECUTABLE=C:\\Users\\Jack\\AppData\\Local\\Programs\\Python\\Python311\\python.exe', '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_RELEASE=C:\\Users\\Jack\\AppData\\Local\\Temp\\pip-install-tl9fdcf0\\dlib_fee2183dfbb9404395bfedaca5728c1a\\build\\lib.win-amd64-cpython-311', '-A', 'x64']' returned non-zero exit status 1.
      [end of output]

  note: This error originates from a subprocess, and is likely not a problem with pip.
  ERROR: Failed building wheel for dlib
Failed to build dlib
ERROR: Could not build wheels for dlib, which is required to
```

- cmake安装
```
 pip install cmake==3.25.2
```

- 根据python版本，下载对应的 dlib whl文件；本地安装
- 安装指令

```
python -m pip install dlib名字.whl
```
- 注意：这些 wheel 文件只能用于在 Windows x64 操作系统上安装 Dlib。



## 📢 New Update:
* May 08, 2024: Added compiled binary file (.whl) for Python 3.12!

## Steps to install Dlib:

* Install Python from [Python.org](https://www.python.org/downloads/) (download the 64-bit installer file)
  
   **OR**
* Create a virtual environment via [venv](https://docs.python.org/3/library/venv.html) or [Anaconda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) i.e. `conda create -n env_name python = 3.8` 
 
* Download the wheel file for your specific Python version 

* Open a terminal and install Dlib via:

### Python 3.7
```
python -m pip install dlib-19.22.99-cp37-cp37m-win_amd64.whl 
```
### Python 3.8
```
python -m pip install dlib-19.22.99-cp38-cp38-win_amd64.whl
```
### Python 3.9
```
python -m pip install dlib-19.22.99-cp39-cp39-win_amd64.whl
```
### Python 3.10
```
python -m pip install dlib-19.22.99-cp310-cp310-win_amd64.whl
```
### Python 3.11
```
python -m pip install dlib-19.24.1-cp311-cp311-win_amd64.whl
```
### Python 3.12
```
python -m pip install dlib-19.24.99-cp312-cp312-win_amd64.whl
```
Cheers!
