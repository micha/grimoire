{% highlight clojure %}
(defn insert-child
  "Inserts the item as the leftmost child of the node at this loc,
  without moving"
  {:added "1.0"}
  [loc item]
    (replace loc (make-node loc (node loc) (cons item (children loc)))))
{% endhighlight %}
