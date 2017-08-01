---
layout: default
---
<div class="columns">
	{% for d in site.data.quotes['data'] %}
		<div class="column col-4">
			<div class="video-responsive">
				<iframe src="https://www.youtube.com/embed/{{ d['youtube-video-id'] }}?start={{ d['start'] }}&end={{ d['end'] }}&vq=small&showinfo=0" frameborder="0" allowfullscreen></iframe>
			</div>
			<blockquote>
				<p>{{ d['quote'] }}</p>
				<cite>{{ d['quotee'] }}</cite>
			</blockquote>
		</div>
	{% endfor %}
</div>