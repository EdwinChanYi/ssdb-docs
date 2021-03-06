# 命令

<div class="alert alert-info">
	命令不区分大小写, 推荐使用小写!
</div>

## Server

---

<div class="commands">
<ul>
	<li data-group="string" data-name="auth">
		<a href="auth.html">
		<span class="command">
			auth
			<span class="args">
			password
			</span>
		</span>
		<span class="summary">向服务器校验访问密码.</span>
		</a>
	</li>
	<li data-group="string" data-name="dbsize">
		<a href="dbsize.html">
		<span class="command">
			dbsize
			<span class="args">
			</span>
		</span>
		<span class="summary">返回数据库占用空间的<code>近似值</code>, 以字节为单位.</span>
		</a>
	</li>
	<li data-group="string" data-name="flushdb">
		<a href="flushdb.html">
		<span class="command">
			flushdb
			<span class="args">
			[type]
			</span>
		</span>
		<span class="summary">删除 SSDB 服务器的所有数据.</span>
		</a>
	</li>
	<li data-group="string" data-name="info">
		<a href="info.html">
		<span class="command">
			info
			<span class="args">
			[opt]
			</span>
		</span>
		<span class="summary">返回服务器的信息.</span>
		</a>
	</li>
</ul>
</div>

## Key Value

---

<div class="commands">
<ul>
	<li data-group="string" data-name="set">
		<a href="set.html">
		<span class="command">
			set
			<span class="args">
			key value
			</span>
		</span>
		<span class="summary">设置指定 key 的值内容.</span>
		</a>
	</li>
	<li data-group="string" data-name="setx">
		<a href="setx.html">
		<span class="command">
			setx
			<span class="args">
			key value ttl
			</span>
		</span>
		<span class="summary">设置指定 key 的值内容, 同时设置存活时间.</span>
		</a>
	</li>
	<li data-group="string" data-name="setnx">
		<a href="setnx.html">
		<span class="command">
			setnx
			<span class="args">
			key value
			</span>
		</span>
		<span class="summary">当 key 不存在时, 设置指定 key 的值内容. 如果已存在, 则不设置.</span>
		</a>
	</li>
	<li data-group="string" data-name="expire">
		<a href="expire.html">
		<span class="command">
			expire
			<span class="args">
			key ttl
			</span>
		</span>
		<span class="summary">设置 key(只针对 KV 类型) 的存活时间.</span>
		</a>
	</li>
	<li data-group="string" data-name="ttl">
		<a href="ttl.html">
		<span class="command">
			ttl
			<span class="args">
			key
			</span>
		</span>
		<span class="summary">返回 key(只针对 KV 类型) 的存活时间.</span>
		</a>
	</li>
	<li data-group="string" data-name="get">
		<a href="get.html">
		<span class="command">
			get
			<span class="args">
			key
			</span>
		</span>
		<span class="summary">获取指定 key 的值内容.</span>
		</a>
	</li>
	<li data-group="string" data-name="getset">
		<a href="getset.html">
		<span class="command">
			getset
			<span class="args">
			key value
			</span>
		</span>
		<span class="summary">更新 key 对应的 value, 并返回更新前的旧的 value.</span>
		</a>
	</li>
	<li data-group="string" data-name="del">
		<a href="del.html">
		<span class="command">
			del
			<span class="args">
			key
			</span>
		</span>
		<span class="summary">删除指定的 key.</span>
		</a>
	</li>
	<li data-group="string" data-name="incr">
		<a href="incr.html">
		<span class="command">
			incr
			<span class="args">
				key [num]
			</span>
		</span>
		<span class="summary">使 key 对应的值增加 num.</span>
		</a>
	</li>
	<li data-group="string" data-name="exists">
		<a href="exists.html">
		<span class="command">
			exists
			<span class="args">
			key
			</span>
		</span>
		<span class="summary">判断指定的 key 是否存在.</span>
		</a>
	</li>
	<li data-group="string" data-name="getbit">
		<a href="getbit.html">
		<span class="command">
			getbit
			<span class="args">
			key offset
			</span>
		</span>
		<span class="summary">获取字符串内指定位置的位值(BIT).</span>
		</a>
	</li>
	<li data-group="string" data-name="setbit">
		<a href="setbit.html">
		<span class="command">
			setbit
			<span class="args">
			key offset val
			</span>
		</span>
		<span class="summary">设置字符串内指定位置的位值(BIT), 字符串的长度会自动扩展.</span>
		</a>
	</li>
	<li data-group="string" data-name="bitcount">
		<a href="bitcount.html">
		<span class="command">
			bitcount
			<span class="args">
			key [start] [end]
			</span>
		</span>
		<span class="summary">计算字符串的子串所包含的位值为 1 的个数.</span>
		</a>
	</li>
	<li data-group="string" data-name="countbit">
		<a href="countbit.html">
		<span class="command">
			countbit
			<span class="args">
			key start size
			</span>
		</span>
		<span class="summary">计算字符串的子串所包含的位值为 1 的个数.</span>
		</a>
	</li>
	<li data-group="string" data-name="substr">
		<a href="substr.html">
		<span class="command">
			substr
			<span class="args">
			key start size
			</span>
		</span>
		<span class="summary">获取字符串的子串.</span>
		</a>
	</li>
	<li data-group="string" data-name="strlen">
		<a href="strlen.html">
		<span class="command">
			strlen
			<span class="args">
			key
			</span>
		</span>
		<span class="summary">计算字符串的长度(字节数).</span>
		</a>
	</li>
	<li data-group="string" data-name="keys">
		<a href="keys.html">
		<span class="command">
			keys
			<span class="args">
				key_start key_end limit
			</span>
		</span>
		<span class="summary">列出处于区间 (key_start, key_end] 的 key 列表.</span>
		</a>
	</li>
	<li data-group="string" data-name="rkeys">
		<a href="rkeys.html">
		<span class="command">
			rkeys
			<span class="args">
				key_start key_end limit
			</span>
		</span>
		<span class="summary">列出处于区间 (key_start, key_end] 的 key 列表, 反向.</span>
		</a>
	</li>
	<li data-group="string" data-name="scan">
		<a href="scan.html">
		<span class="command">
			scan
			<span class="args">
				key_start key_end limit
			</span>
		</span>
		<span class="summary">列出处于区间 (key_start, key_end] 的 key-value 列表.</span>
		</a>
	</li>
	<li data-group="string" data-name="rscan">
		<a href="rscan.html">
		<span class="command">
			rscan
			<span class="args">
				key_start key_end limit
			</span>
		</span>
		<span class="summary">列出处于区间 (key_start, key_end] 的 key-value 列表, 反向.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_set">
		<a href="multi_set.html">
		<span class="command">
			multi_set
			<span class="args">
			key1 value1 key2 value2 ...
			</span>
		</span>
		<span class="summary">批量设置一批 key-value.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_get">
		<a href="multi_get.html">
		<span class="command">
			multi_get
			<span class="args">
			key1 key2 ...
			</span>
		</span>
		<span class="summary">批量获取一批 key 对应的值内容.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_del">
		<a href="multi_del.html">
		<span class="command">
			multi_del
			<span class="args">
			key1 key2 ...
			</span>
		</span>
		<span class="summary">批量删除一批 key 和其对应的值内容.</span>
		</a>
	</li>
</ul>
</div>

## Hashmap

---

<div class="commands">
<ul>
	<li data-group="string" data-name="hset">
		<a href="hset.html">
		<span class="command">
			hset
			<span class="args">
			name key value
			</span>
		</span>
		<span class="summary">设置 hashmap 中指定 key 对应的值内容.</span>
		</a>
	</li>
	<li data-group="string" data-name="hget">
		<a href="hget.html">
		<span class="command">
			hget
			<span class="args">
			name key
			</span>
		</span>
		<span class="summary">获取 hashmap 中指定 key 的值内容.</span>
		</a>
	</li>
	<li data-group="string" data-name="hdel">
		<a href="hdel.html">
		<span class="command">
			hdel
			<span class="args">
			name key
			</span>
		</span>
		<span class="summary">获取 hashmap 中的指定 key.</span>
		</a>
	</li>
	<li data-group="string" data-name="hincr">
		<a href="hincr.html">
		<span class="command">
			hincr
			<span class="args">
				name key [num]
			</span>
		</span>
		<span class="summary">使 hashmap 中的 key 对应的值增加 num.</span>
		</a>
	</li>
	<li data-group="string" data-name="hexists">
		<a href="hexists.html">
		<span class="command">
			hexists
			<span class="args">
			name key
			</span>
		</span>
		<span class="summary">判断指定的 key 是否存在于 hashmap 中.</span>
		</a>
	</li>
	<li data-group="string" data-name="hsize">
		<a href="hsize.html">
		<span class="command">
			hsize
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">返回 hashmap 中的元素个数.</span>
		</a>
	</li>
	<li data-group="string" data-name="hlist">
		<a href="hlist.html">
		<span class="command">
			hlist
			<span class="args">
				name_start name_end limit
			</span>
		</span>
		<span class="summary">列出名字处于区间 (name_start, name_end] 的 hashmap.</span>
		</a>
	</li>
	<li data-group="string" data-name="hrlist">
		<a href="hrlist.html">
		<span class="command">
			hrlist
			<span class="args">
				name_start name_end limit
			</span>
		</span>
		<span class="summary">像 hrlist, 逆序.</span>
		</a>
	</li>
	<li data-group="string" data-name="hkeys">
		<a href="hkeys.html">
		<span class="command">
			hkeys
			<span class="args">
				name key_start key_end
			</span>
		</span>
		<span class="summary">列出 hashmap 中处于区间 (key_start, key_end] 的 key 列表.</span>
		</a>
	</li>
	<li data-group="string" data-name="hgetall">
		<a href="hgetall.html">
		<span class="command">
			hgetall
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">返回整个 hashmap.</span>
		</a>
	</li>
	<li data-group="string" data-name="hscan">
		<a href="hscan.html">
		<span class="command">
			hscan
			<span class="args">
				name key_start key_end limit
			</span>
		</span>
		<span class="summary">列出 hashmap 中处于区间 (key_start, key_end] 的 key-value 列表.</span>
		</a>
	</li>
	<li data-group="string" data-name="hrscan">
		<a href="hrscan.html">
		<span class="command">
			hrscan
			<span class="args">
				name key_start key_end limit
			</span>
		</span>
		<span class="summary">像 hscan, 逆序.</span>
		</a>
	</li>
	<li data-group="string" data-name="hclear">
		<a href="hclear.html">
		<span class="command">
			hclear
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">删除 hashmap 中的所有 key.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_hset">
		<a href="multi_hset.html">
		<span class="command">
			multi_hset
			<span class="args">
			name key1 value1 key2 value2 ...
			</span>
		</span>
		<span class="summary">批量设置 hashmap 中的 key-value.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_hget">
		<a href="multi_hget.html">
		<span class="command">
			multi_hget
			<span class="args">
			name key1 key2 ...
			</span>
		</span>
		<span class="summary">批量获取 hashmap 中多个 key 对应的权重值.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_hdel">
		<a href="multi_hdel.html">
		<span class="command">
			multi_hdel
			<span class="args">
			name key1 key2 ...
			</span>
		</span>
		<span class="summary">指删除 hashmap 中的 key.</span>
		</a>
	</li>
</ul>
</div>

## Sorted Set

---

<div class="commands">
<ul>
	<li data-group="string" data-name="zset">
		<a href="zset.html">
		<span class="command">
			zset
			<span class="args">
			name key score
			</span>
		</span>
		<span class="summary">设置 zset 中指定 key 对应的权重值.</span>
		</a>
	</li>
	<li data-group="string" data-name="zget">
		<a href="zget.html">
		<span class="command">
			zget
			<span class="args">
			name key
			</span>
		</span>
		<span class="summary">获取 zset 中指定 key 的权重值.</span>
		</a>
	</li>
	<li data-group="string" data-name="zdel">
		<a href="zdel.html">
		<span class="command">
			zdel
			<span class="args">
			name key
			</span>
		</span>
		<span class="summary">获取 zset 中的指定 key.</span>
		</a>
	</li>
	<li data-group="string" data-name="zincr">
		<a href="zincr.html">
		<span class="command">
			zincr
			<span class="args">
			name key num
			</span>
		</span>
		<span class="summary">使 zset 中的 key 对应的值增加 num. 参数 num 可以为负数. 如果原来的值不是整数(字符串形式的整数), 它会被先转换成整数.</span>
		</a>
	</li>
	<li data-group="string" data-name="zexists">
		<a href="zexists.html">
		<span class="command">
			zexists
			<span class="args">
			name key
			</span>
		</span>
		<span class="summary">判断指定的 key 是否存在于 zset 中.</span>
		</a>
	</li>
	<li data-group="string" data-name="zsize">
		<a href="zsize.html">
		<span class="command">
			zsize
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">返回 zset 中的元素个数.</span>
		</a>
	</li>
	<li data-group="string" data-name="zlist">
		<a href="zlist.html">
		<span class="command">
			zlist
			<span class="args">
			</span>
		</span>
		<span class="summary">列出名字处于区间 (name_start, name_end] 的 zset.</span>
		</a>
	</li>
	<li data-group="string" data-name="zrlist">
		<a href="zrlist.html">
		<span class="command">
			zrlist
			<span class="args">
			</span>
		</span>
		<span class="summary">像 zlist, 逆序.</span>
		</a>
	</li>
	<li data-group="string" data-name="zkeys">
		<a href="zkeys.html">
		<span class="command">
			zkeys
			<span class="args">
				name key_start score_start score_end limit
			</span>
		</span>
		<span class="summary">列出 zset 中的 key 列表.</span>
		</a>
	</li>
	<li data-group="string" data-name="zscan">
		<a href="zscan.html">
		<span class="command">
			zscan
			<span class="args">
				name key_start score_start score_end limit
			</span>
		</span>
		<span class="summary">列出 zset 中处于区间 (key_start+score_start, score_end] 的 key-score 列表.</span>
		</a>
	</li>
	<li data-group="string" data-name="zrscan">
		<a href="zrscan.html">
		<span class="command">
			zrscan
			<span class="args">
				name key_start score_start score_end limit
			</span>
		</span>
		<span class="summary">像 zscan, 逆序.</span>
		</a>
	</li>
	<li data-group="string" data-name="zrank">
		<a href="zrank.html">
		<span class="command">
			zrank
			<span class="args">
				name key
			</span>
		</span>
		<span class="summary">返回指定 key 在 zset 中的排序位置(排名), 排名从 0 开始.</span>
		</a>
	</li>
	<li data-group="string" data-name="zrrank">
		<a href="zrrank.html">
		<span class="command">
			zrrank
			<span class="args">
				name key
			</span>
		</span>
		<span class="summary">像 zrank, 逆序.</span>
		</a>
	</li>
	<li data-group="string" data-name="zrange, zrrange">
		<a href="zrange.html">
		<span class="command">
			zrange
			<span class="args">
				name offset limit
			</span>
		</span>
		<span class="summary">根据下标索引区间 [offset, offset + limit) 获取 key-score 对, 下标从 0 开始.</span>
		</a>
	</li>
	<li data-group="string" data-name="zrrange">
		<a href="zrrange.html">
		<span class="command">
			zrrange
			<span class="args">
				name offset limit
			</span>
		</span>
		<span class="summary">像 zrange, 逆序.</span>
		</a>
	</li>
	<li data-group="string" data-name="zclear">
		<a href="zclear.html">
		<span class="command">
			zclear
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">删除 zset 中的所有 key.</span>
		</a>
	</li>
	<li data-group="string" data-name="zcount">
		<a href="zcount.html">
		<span class="command">
			zcount
			<span class="args">
				name start end
			</span>
		</span>
		<span class="summary">返回处于区间 [start,end] key 数量.</span>
		</a>
	</li>
	<li data-group="string" data-name="zsum">
		<a href="zsum.html">
		<span class="command">
			zsum
			<span class="args">
				name start end
			</span>
		</span>
		<span class="summary">返回 key 处于区间 [start,end] 的 score 的和.</span>
		</a>
	</li>
	<li data-group="string" data-name="zavg">
		<a href="zavg.html">
		<span class="command">
			zavg
			<span class="args">
				name start end
			</span>
		</span>
		<span class="summary">返回 key 处于区间 [start,end] 的 score 的平均值.</span>
		</a>
	</li>
	<li data-group="string" data-name="zremrangebyrank">
		<a href="zremrangebyrank.html">
		<span class="command">
			zremrangebyrank
			<span class="args">
				name start end
			</span>
		</span>
		<span class="summary">删除位置处于区间 [start,end] 的元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="zremrangebyscore">
		<a href="zremrangebyscore.html">
		<span class="command">
			zremrangebyscore
			<span class="args">
				name start end
			</span>
		</span>
		<span class="summary">删除权重处于区间 [start,end] 的元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="zpop_front">
		<a href="zpop_front.html">
		<span class="command">
			zpop_front
			<span class="args">
				name limit
			</span>
		</span>
		<span class="summary">从 zset 首部删除 <code>limit</code> 个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="zpop_back">
		<a href="zpop_back.html">
		<span class="command">
			zpop_back
			<span class="args">
				name limit
			</span>
		</span>
		<span class="summary">从 zset 尾部删除 <code>limit</code> 个元素.</span>
	</li>
	<li data-group="string" data-name="multi_zset">
		<a href="multi_zset.html">
		<span class="command">
			multi_zset
			<span class="args">
			name key1 score1 key2 score2 ...
			</span>
		</span>
		<span class="summary">批量设置 zset 中的 key-score.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_zget">
		<a href="multi_zget.html">
		<span class="command">
			multi_zget
			<span class="args">
			name key1 key2 ...
			</span>
		</span>
		<span class="summary">批量获取 zset 中多个 key 对应的权重值.</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_zdel">
		<a href="multi_zdel.html">
		<span class="command">
			multi_zdel
			<span class="args">
			name key1 key2 ...
			</span>
		</span>
		<span class="summary">批量删除 zset 中的 key.</span>
		</a>
	</li>

</ul>
</div>



## List

---

<div class="commands">
<ul>
	<li data-group="string" data-name="qpush_front">
		<a href="qpush_front.html">
		<span class="command">
			qpush_front
			<span class="args">
			name item1 item2 ...
			</span>
		</span>
		<span class="summary">往队列的首部添加一个或者多个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qpush_back">
		<a href="qpush_back.html">
		<span class="command">
			qpush_back
			<span class="args">
			name item1 item2 ...
			</span>
		</span>
		<span class="summary">往队列的尾部添加一个或者多个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qpop_front">
		<a href="qpop_front.html">
		<span class="command">
			qpop_front
			<span class="args">
			name size
			</span>
		</span>
		<span class="summary">从队列首部弹出最后一个或者多个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qpop_back">
		<a href="qpop_back.html">
		<span class="command">
			qpop_back
			<span class="args">
			name size
			</span>
		</span>
		<span class="summary">从队列尾部弹出最后一个或者多个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qpush">
		<a href="qpush.html">
		<span class="command">
			qpush
			<span class="args">
				name item1 item2 ...
			</span>
		</span>
		<span class="summary">是 `qpush_back` 的别名.. </span>
		</a>
	</li>
	<li data-group="string" data-name="qpop">
		<a href="qpop.html">
		<span class="command">
			qpop
			<span class="args">
			name size
			</span>
		</span>
		<span class="summary">是 `qpop_front` 的别名.. </span>
		</a>
	</li>
	<li data-group="string" data-name="qfront">
		<a href="qfront.html">
		<span class="command">
			qfront
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">返回队列的第一个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qback">
		<a href="qback.html">
		<span class="command">
			qback
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">返回队列的最后一个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qsize">
		<a href="qsize.html">
		<span class="command">
			qsize
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">返回队列的长度.</span>
		</a>
	</li>
	<li data-group="string" data-name="qclear">
		<a href="qclear.html">
		<span class="command">
			qclear
			<span class="args">
			name
			</span>
		</span>
		<span class="summary">清空一个队列.</span>
		</a>
	</li>
	<li data-group="string" data-name="qget">
		<a href="qget.html">
		<span class="command">
			qget
			<span class="args">
			name index
			</span>
		</span>
		<span class="summary">返回指定位置的元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qset">
		<a href="qset.html">
		<span class="command">
			qset
			<span class="args">
				name index val
			</span>
		</span>
		<span class="summary">更新位于 index 位置的元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qrange">
		<a href="qrange.html">
		<span class="command">
			qrange
			<span class="args">
			name offset limit
			</span>
		</span>
		<span class="summary">返回下标处于区域 [offset, offset + limit] 的元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qslice">
		<a href="qslice.html">
		<span class="command">
			qslice
			<span class="args">
			name begin end
			</span>
		</span>
		<span class="summary">返回下标处于区域 [begin, end] 的元素. begin 和 end 可以是负数</span>
		</a>
	</li>
	<li data-group="string" data-name="qtrim_front">
		<a href="qtrim_front.html">
		<span class="command">
			qtrim_front
			<span class="args">
			name size
			</span>
		</span>
		<span class="summary">从队列头部删除多个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qtrim_back">
		<a href="qtrim_back.html">
		<span class="command">
			qtrim_back
			<span class="args">
			name size
			</span>
		</span>
		<span class="summary">从队列头部删除多个元素.</span>
		</a>
	</li>
	<li data-group="string" data-name="qlist">
		<a href="qlist.html">
		<span class="command">
			qlist
			<span class="args">
				name_start name_end limit
			</span>
		</span>
		<span class="summary">列出名字处于区间 (name_start, name_end] 的 queue/list.</span>
		</a>
	</li>
	<li data-group="string" data-name="qrlist">
		<a href="qrlist.html">
		<span class="command">
			qrlist
			<span class="args">
				name_start name_end limit
			</span>
		</span>
		<span class="summary">像 qlist, 逆序.</span>
		</a>
	</li>

</ul>
</div>
