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
		<span class="summary">Get the value related to the specified key</span>
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
		<span class="summary">Sets a value and returns the previous entry at that key.</span>
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
		<span class="summary">Delete specified key.</span>
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
		<span class="summary">Increment the number stored at key by num.</span>
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
		<span class="summary">Verify if the specified key exists.</span>
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
		<span class="summary">Return a single bit out of a string.</span>
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
		<span class="summary">Changes a single bit of a string. The string is auto expanded.</span>
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
		<span class="summary">Count the number of set bits (population counting) in part of a string.</span>
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
		<span class="summary">Count the number of set bits (population counting) in part of a string.</span>
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
		<span class="summary">Return part of a string.</span>
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
		<span class="summary">Return the number of bytes of a string.</span>
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
		<span class="summary">List keys in range (key_start, key_end].</span>
		</a>
	</li>
	<li data-group="string" data-name="keys">
		<a href="keys.html">
		<span class="command">
			rkeys
			<span class="args">
				key_start key_end limit
			</span>
		</span>
		<span class="summary">List keys in range (key_start, key_end], in reverse order.</span>
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
		<span class="summary">List key-value pairs with keys in range (key_start, key_end].</span>
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
		<span class="summary">List key-value pairs with keys in range (key_start, key_end], in reverse order.</span>
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
		<span class="summary">Set multiple key-value pairs(kvs) in one method call.</span>
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
		<span class="summary">Get the values related to the specified multiple keys</span>
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
		<span class="summary">Delete specified multiple keys.</span>
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
		<span class="summary">Set the string value in argument as value of the key of a hashmap.</span>
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
		<span class="summary">Get the value related to the specified key of a hashmap</span>
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
		<span class="summary">Delete specified key of a hashmap.</span>
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
		<span class="summary">Increment the number stored at key in a hashmap by num</span>
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
		<span class="summary">Verify if the specified key exists in a hashmap.</span>
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
		<span class="summary">Return the number of key-value pairs in the hashmap.</span>
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
		<span class="summary">List hashmap names in range (name_start, name_end].</span>
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
		<span class="summary">List hashmap names in range (name_start, name_end].</span>
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
		<span class="summary">List keys of a hashmap in range (key_start, key_end].</span>
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
		<span class="summary">Returns the whole hash, as an array of strings indexed by strings.</span>
		</a>
	</li>
	<li data-group="string" data-name="hscan">
		<a href="hscan.html">
		<span class="command">
			hscan
			<span class="args">
				key_start key_end limit
			</span>
		</span>
		<span class="summary">List key-value pairs of a hashmap with keys in range (key_start, key_end].</span>
		</a>
	</li>
	<li data-group="string" data-name="hrscan">
		<a href="hrscan.html">
		<span class="command">
			hrscan
			<span class="args">
				key_start key_end limit
			</span>
		</span>
		<span class="summary">List key-value pairs with keys in range (key_start, key_end], in reverse order.</span>
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
		<span class="summary">Delete all keys in a hashmap.</span>
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
		<span class="summary">Set multiple key-value pairs(kvs) of a hashmap in one method call.</span>
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
		<span class="summary">Get the values related to the specified multiple keys of a hashmap.</span>
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
		<span class="summary">Delete specified multiple keys in a hashmap.</span>
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
		<span class="summary">Set the score of the key of a zset.</span>
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
		<span class="summary">Get the score related to the specified key of a zset</span>
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
		<span class="summary">Delete specified key of a zset.</span>
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
		<span class="summary">Increment the number stored at key in a zset by num.</span>
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
		<span class="summary">Verify if the specified key exists in a zset.</span>
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
		<span class="summary">Return the number of pairs of a zset.</span>
		</a>
	</li>
	<li data-group="string" data-name="zlist">
		<a href="zlist.html">
		<span class="command">
			zlist
			<span class="args">
			</span>
		</span>
		<span class="summary">List zset names in range (name_start, name_end].</span>
		</a>
	</li>
	<li data-group="string" data-name="zrlist">
		<a href="zrlist.html">
		<span class="command">
			zrlist
			<span class="args">
			</span>
		</span>
		<span class="summary">List zset names in range (name_start, name_end], in reverse order.</span>
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
		<span class="summary">List keys in a zset.</span>
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
		<span class="summary">List key-score pairs where key-score in range (key_start+score_start, score_end].</span>
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
		<span class="summary">List key-score pairs of a zset, in reverse order. See method zkeys().</span>
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
		<span class="summary">Returns the rank(index) of a given key in the specified sorted set.</span>
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
		<span class="summary">Returns the rank(index) of a given key in the specified sorted set, in reverse order.</span>
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
		<span class="summary">Returns a range of key-score pairs by index range [offset, offset + limit).</span>
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
		<span class="summary">Returns a range of key-score pairs by index range [offset, offset + limit), in reverse order.</span>
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
		<span class="summary">Delete all keys in a zset.</span>
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
		<span class="summary">Returns the number of elements of the sorted set stored at the specified key.</span>
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
		<span class="summary">Returns the sum of elements of the sorted set stored at the specified key.</span>
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
		<span class="summary">Returns the average of elements of the sorted set stored at the specified key.</span>
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
		<span class="summary">Delete the elements of the zset which have rank in the range [start,end].</span>
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
		<span class="summary">Delete the elements of the zset which have score in the range [start,end].</span>
		</a>
	</li>
	<li data-group="string" data-name="multi_zset">
		<a href="multi_zset.html">
		<span class="command">
			multi_zset
			<span class="args">
			name key1 score1 key2 score2 ...
			</span>
		</span>
		<span class="summary">Set multiple key-score pairs(kvs) of a zset in one method call.</span>
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
		<span class="summary">Get the values related to the specified multiple keys of a zset.</span>
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
		<span class="summary">Delete specified multiple keys of a zset.</span>
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
		<span class="summary">Adds one or more than one element to the head of the queue.</span>
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
		<span class="summary">Adds an or more than one element to the end of the queue.</span>
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
		<span class="summary">Pop out one or more elements from the head of a queue.</span>
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
		<span class="summary">Pop out one or more elements from the tail of a queue.</span>
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
		<span class="summary">Alias of `qpush_front`. </span>
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
		<span class="summary">Alias of `qpop_front`. </span>
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
		<span class="summary">Returns the first element of a queue.</span>
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
		<span class="summary">Returns the last element of a queue.</span>
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
		<span class="summary">Returns the number of items in the queue.</span>
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
		<span class="summary">Clear the queue.</span>
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
		<span class="summary">Returns the element a the specified index(position).</span>
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
		<span class="summary">Description</span>
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
		<span class="summary">Returns a portion of elements from the queue at the specified range [offset, offset + limit].</span>
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
		<span class="summary">Returns a portion of elements from the queue at the specified range [begin, end].</span>
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
		<span class="summary">Remove multi elements from the head of a queue.</span>
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
		<span class="summary">Remove multi elements from the tail of a queue.</span>
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
		<span class="summary">List list/queue names in range (name_start, name_end].</span>
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
		<span class="summary">List list/queue names in range (name_start, name_end], in reverse order.</span>
		</a>
	</li>

</ul>
</div>
