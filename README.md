# convert_to_py for Pyqt

Pyqt에서 Qt designer를 사용하면 생성되는 .qrc 파일들 및 .ui 파일들을 .py로 변환하는 파이썬 프로그램입니다.

.qrc 파일만 변환하거나 .ui 파일만 변환하거나 아니면 둘 다 변환하는 것을 선택할 수 있습니다. 

.qrc 파일 경로의 개수와 위치는 상관없으며 입력한 순서대로 변환됩니다. 변환 위치는 본래 .qrc 파일과 같은 경로에 변환되며 본래 .qrc 파일의 이름에 \_rc가 추가됩니다.

.ui 파일을 변환할 때 변환된 파일이 위치할 경로를 입력하지 않으면 .ui 파일 경로와 같은 위치로 변환됩니다. 변환된 .ui의 .py파일의 이름은 본래 .ui 파일의 이름에 \_ui가 추가됩니다.

## Run and Usage

```
$ python convert_to_py.py
Usage is ...
	python convert_to_py.py [RESOURCE FILES PATH ...]
	python convert_to_py.py [UI FILES DIR PATH]
	python convert_to_py.py [UI FILES DIR PATH] [PY FILES DIR PATH]
	python convert_to_py.py [RESOURCE FILES PATH ...] [UI FILES DIR PATH] [PY FILES DIR PATH]

$ python convert_to_py.py resources.qrc designer package/ui
Converted: resources.qrc -> resources_rc.py
Converted: designer/test.ui -> package/ui/test_ui.py
```

## License

`convert_to_py for Pyqt` for is primarily distributed under the terms of MIT license.

See [LICENSE](./LICENSE) for details.