Ansj中文分词 for lucene4
=========================

<pre><code>
Ansj索引时采用面向索引的分词：我在首都机场虹桥路滑旱冰！玩的很Happy，很Hi！
1: [我:0->1:word] 
2: [在:1->2:word] 
3: [首都机场:2->6:word] 
4: [虹桥:6->8:word] 
5: [虹桥路:6->9:word] 
6: [路:8->9:word] 
7: [滑:9->10:word] 
8: [滑旱冰:9->12:word] 
9: [旱冰:10->12:word] 
10: [！:12->13:word] 
11: [玩:13->14:word] 
12: [的:14->15:word] 
13: [很:15->16:word] 
14: [happy:16->21:word] 
15: [，:21->22:word] 
16: [很:22->23:word] 
17: [hi:23->25:word] 
18: [！:25->26:word] 
索引分词时过滤停用词
3: [首都机场:2->6:word] 
4: [虹桥:6->8:word] 
5: [虹桥路:6->9:word] 
6: [路:8->9:word] 
7: [滑:9->10:word] 
8: [滑旱冰:9->12:word] 
9: [旱冰:10->12:word] 
11: [玩:13->14:word] 
13: [很:15->16:word] 
14: [happy:16->21:word] 
16: [很:22->23:word] 
17: [hi:23->25:word] 
------------------------------------------------------------
Ansj查询时采用精准分词：我在首都机场虹桥路滑旱冰！玩的很Happy，很Hi！
1: [我:0->1:word] 
2: [在:1->2:word] 
3: [首都机场:2->6:word] 
4: [虹桥路:6->9:word] 
5: [滑旱冰:9->12:word] 
6: [！:12->13:word] 
7: [玩:13->14:word] 
8: [的:14->15:word] 
9: [很:15->16:word] 
10: [happy:16->21:word] 
11: [，:21->22:word] 
12: [很:22->23:word] 
13: [hi:23->25:word] 
14: [！:25->26:word] 
查询分词时过滤停用词
3: [首都机场:2->6:word] 
4: [虹桥路:6->9:word] 
5: [滑旱冰:9->12:word] 
7: [玩:13->14:word] 
9: [很:15->16:word] 
10: [happy:16->21:word] 
12: [很:22->23:word] 
13: [hi:23->25:word]
</code></pre> 