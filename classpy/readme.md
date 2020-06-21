# class の使い方について
## with 構文が使用できるクラス
```
class Stove():

    def __init__(self):
        self.switch = False

    def switch_on(self):
        if not self.switch:
            self.switch = True
            print('コンロ点火しました')

    def switch_off(self):
        if self.switch:
            self.switch = False
            print('コンロ消化しました')

    def boil(self, stuff):
        print('%sを茹でました。' % stuff)

    def __enter__(self):
        self.switch_on()
        return self

    def __exit__(self, exception_type, exception_value, traceback):
        self.switch_off()
```


# 参考

[[Python] with 構文で使用できるクラスを実装する](https://qiita.com/tchnkmr/items/c6b6480d236a51b91c17)
[Python のクラスにおける**call**メソッドの使い方](https://qiita.com/ko-da-k/items/439d8cc3a0424c45214a)
