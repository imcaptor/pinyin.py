pinyin.py
=========

汉字转拼音,With Python

1.修正中文中有英文字母或者数字的bug
2.修正分隔符为空的bug


Example:

    from pinyin import PinYin
    
    test = PinYin()
    test.load_word()
    test.hanzi2pinyin(string='钓鱼岛是中国的')


Out:

    test.hanzi2pinyin(string='钓鱼岛是中国的')
    ['diao', 'yu', 'dao', 'shi', 'zhong', 'guo', 'de']    
    test.hanzi2pinyin_split(string='钓鱼岛是中国的', split="-")
    diao-yu-dao-shi-zhong-guo-de
    test.hanzi2pinyin_split(string='钓鱼岛是a中国的', split="")
    diaoyudaoshiazhongguode

