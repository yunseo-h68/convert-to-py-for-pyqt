# convert_to_py for Pyqt

Pyqt에서 Qt designer를 사용하면 생성되는 .qrc 파일들 및 .ui 파일들을 .py로 변환합니다.

convert_qrc_to_py.py는 .qrc 파일들을 변환하고 convert_ui_to_py.py는 .ui 파일들을 변환합니다.

.ui, .qrc 파일들을 변환할 때 변환된 파일이 위치할 경로를 입력하지 않으면 .ui, .qrc 파일 경로와 같은 위치로 변환됩니다. 변환된 .py 파일의 이름은 .qrc 파일은 \_rc가, .ui 파일은 \_ui가 추가됩니다.

## Run and Usage

```
$ python convert_qrc_to_py.py
Usage is ...
    python convert_qrc_to_py.py [RESOURCE FILES DIR PATH]
    python convert_qrc_to_py.py [RESOURCE FILES DIR PATH] [PY FILES DIR PATH]

$ python convert_qrc_to_py.py . package/ui
Converted: resources.qrc -> resources_rc.py

$ python convert_ui_to_py.py
Usage is ...
    python convert_ui_to_py.py [UI FILES DIR PATH]
    python convert_ui_to_py.py [UI FILES DIR PATH] [PY FILES DIR PATH]

$ python convert_ui_to_py.py designer package/ui
Converted: designer/test.ui -> package/ui/test_ui.py
```

## License

`convert_to_py for Pyqt` for is primarily distributed under the terms of MIT license.

See [LICENSE](./LICENSE) for details.