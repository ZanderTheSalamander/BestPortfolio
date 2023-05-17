<script>
	import Testimonial from '$lib/components/testimonial/Testimonial.svelte';
</script>


<section class='bg-neutral-100 w-full flex place-content-center py-10'>
	<div class='grid grid-cols-3 md:grid-cols-3 gap-4 w-3/4'>
		<Testimonial
			company='ACADIA OUTDOORS'
			logo='https://images-platform.99static.com//K-BoBDy9Y9ac-QRVUXR6TFnLjQA=/318x327:1663x1672/fit-in/500x500/99designs-contests-attachments/114/114990/attachment_114990855'
			name='John Lowe'
			quote='Quote Placeholder'
			role='CEO'
		/>
		<Testimonial
			company='Company'
			logo='https://picsum.photos/200/300'
			name='John Doe'
			quote='Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac libero eu
  odio rutrum aliquam. Nullam eget massa euismod, ullamcorper massa quis,
  ultricies quam. Sed ac libero eu odio rutrum aliquam. Nullam eget massa
  euismod, ullamcorper massa quis, ultricies quam.'
			role='CEO'
		/>
		<Testimonial
			company='Company'
			logo='https://picsum.photos/200/300'
			name='John Doe'
			quote='Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac libero eu
  odio rutrum aliquam. Nullam eget massa euismod, ullamcorper massa quis,
  ultricies quam. Sed ac libero eu odio rutrum aliquam. Nullam eget massa
  euismod, ullamcorper massa quis, ultricies quam.'
			role='CEO'
		/>
	</div>
</section>