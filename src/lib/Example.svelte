<script lang="ts">
	import type { Snippet } from "svelte";

	let { foo } = $props<{ foo: Snippet<[string]> }>();

	function bar() {
		return "baz";
	}
</script>

{@render foo(bar())}
