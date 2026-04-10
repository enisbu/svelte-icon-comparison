<script lang="ts">
	import {
		Home as LucideHome,
		Search as LucideSearch,
		Settings as LucideSettings,
		Heart as LucideHeart,
		Star as LucideStar,
		Calendar as LucideCalendar,
		Mail as LucideMail,
		Phone as LucidePhone,
		Camera as LucideCamera,
		ChevronRight as LucideChevronRight
	} from '@lucide/svelte';

	import {
		IconHome,
		IconSearch,
		IconSettings,
		IconHeart,
		IconStar,
		IconCalendar,
		IconMail,
		IconPhone,
		IconCamera,
		IconChevronRight,
		IconBrandInstagram,
		IconBrandWhatsapp,
		IconBrandGithub,
		IconBrandTwitter,
		IconBrandTiktok
	} from '@tabler/icons-svelte';

	import {
		House as PhosphorHouse,
		MagnifyingGlass as PhosphorSearch,
		Gear as PhosphorGear,
		Heart as PhosphorHeart,
		Star as PhosphorStar,
		Calendar as PhosphorCalendar,
		Envelope as PhosphorEnvelope,
		Phone as PhosphorPhone,
		Camera as PhosphorCamera,
		CaretRight as PhosphorCaretRight,
		InstagramLogo as PhosphorInstagram,
		WhatsappLogo as PhosphorWhatsapp,
		GithubLogo as PhosphorGithub,
		XLogo as PhosphorX,
		TiktokLogo as PhosphorTiktok
	} from 'phosphor-svelte';

	import {
		HomeLineBuildings as RemixHome,
		SearchLineSystem as RemixSearch,
		Settings3LineSystem as RemixSettings,
		HeartLineHealthMedical as RemixHeart,
		StarLineSystem as RemixStar,
		CalendarLineBusiness as RemixCalendar,
		MailLineBusiness as RemixMail,
		PhoneLineDevice as RemixPhone,
		CameraLineMedia as RemixCamera,
		ArrowRightSLineArrows as RemixChevronRight,
		InstagramLineLogos as RemixInstagram,
		WhatsappLineLogos as RemixWhatsapp,
		GithubLineLogos as RemixGithub,
		TwitterLineLogos as RemixTwitter,
		TiktokLineLogos as RemixTiktok
	} from 'svelte-remix';

	import { HugeiconsIcon } from '@hugeicons/svelte';
	import {
		Home01Icon,
		Search01Icon,
		Settings01Icon,
		FavouriteIcon,
		StarIcon,
		Calendar01Icon,
		Mail01Icon,
		TelephoneIcon,
		Camera01Icon,
		ArrowRight01Icon,
		InstagramIcon,
		WhatsappIcon,
		GithubIcon,
		TwitterIcon,
		TiktokIcon
	} from '@hugeicons/core-free-icons';

	import IconCell from '$lib/IconCell.svelte';

	const SIZE = 24;
</script>

<svelte:head>
	<title>Icon Library Comparison</title>
</svelte:head>

<div class="min-h-screen bg-zinc-950 text-zinc-100 px-6 py-12 font-sans">
	<div class="mx-auto max-w-7xl">
		<header class="mb-16 text-center">
			<h1 class="text-4xl font-bold tracking-tight text-white sm:text-5xl">
				Svelte Icon Libraries
			</h1>
			<p class="mt-4 text-lg text-zinc-400">
				Side-by-side comparison of 5 popular icon packages for Svelte 5
			</p>
		</header>

		<div class="grid gap-8">

			<!-- LUCIDE -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8">
				<div class="mb-6 flex flex-wrap items-baseline gap-x-6 gap-y-2">
					<h2 class="text-2xl font-semibold text-white">@lucide/svelte</h2>
					<span class="rounded-full bg-emerald-500/10 px-3 py-0.5 text-sm text-emerald-400">v1.8.0</span>
				</div>

				<div class="mb-6 grid grid-cols-2 gap-4 text-sm text-zinc-400 sm:grid-cols-4">
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Icons</span>
						<span class="text-zinc-200">~1,500+</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Brand Icons</span>
						<span class="text-red-400">No</span>
						<span class="block text-xs text-zinc-500">Brand icons removed in v1.x</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Tree-shakeable</span>
						<span class="text-emerald-400">Yes</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Bundle per icon</span>
						<span class="text-zinc-200">~1 KB</span>
					</div>
				</div>

				<div class="mb-4">
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Common Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Home"><LucideHome size={SIZE} /></IconCell>
						<IconCell label="Search"><LucideSearch size={SIZE} /></IconCell>
						<IconCell label="Settings"><LucideSettings size={SIZE} /></IconCell>
						<IconCell label="Heart"><LucideHeart size={SIZE} /></IconCell>
						<IconCell label="Star"><LucideStar size={SIZE} /></IconCell>
						<IconCell label="Calendar"><LucideCalendar size={SIZE} /></IconCell>
						<IconCell label="Mail"><LucideMail size={SIZE} /></IconCell>
						<IconCell label="Phone"><LucidePhone size={SIZE} /></IconCell>
						<IconCell label="Camera"><LucideCamera size={SIZE} /></IconCell>
						<IconCell label="ChevronRight"><LucideChevronRight size={SIZE} /></IconCell>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Instagram" disabled />
						<IconCell label="WhatsApp" disabled />
						<IconCell label="Github" disabled />
						<IconCell label="Twitter/X" disabled />
						<IconCell label="TikTok" disabled />
					</div>
				</div>
			</section>

			<!-- TABLER -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8">
				<div class="mb-6 flex flex-wrap items-baseline gap-x-6 gap-y-2">
					<h2 class="text-2xl font-semibold text-white">@tabler/icons-svelte</h2>
					<span class="rounded-full bg-blue-500/10 px-3 py-0.5 text-sm text-blue-400">v3.41.1</span>
				</div>

				<div class="mb-6 grid grid-cols-2 gap-4 text-sm text-zinc-400 sm:grid-cols-4">
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Icons</span>
						<span class="text-zinc-200">~5,800+</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Brand Icons</span>
						<span class="text-emerald-400">Yes</span>
						<span class="block text-xs text-zinc-500">Instagram, WhatsApp, Github, Twitter, TikTok</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Tree-shakeable</span>
						<span class="text-emerald-400">Yes</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Bundle per icon</span>
						<span class="text-zinc-200">~1-2 KB</span>
					</div>
				</div>

				<div class="mb-4">
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Common Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Home"><IconHome size={SIZE} /></IconCell>
						<IconCell label="Search"><IconSearch size={SIZE} /></IconCell>
						<IconCell label="Settings"><IconSettings size={SIZE} /></IconCell>
						<IconCell label="Heart"><IconHeart size={SIZE} /></IconCell>
						<IconCell label="Star"><IconStar size={SIZE} /></IconCell>
						<IconCell label="Calendar"><IconCalendar size={SIZE} /></IconCell>
						<IconCell label="Mail"><IconMail size={SIZE} /></IconCell>
						<IconCell label="Phone"><IconPhone size={SIZE} /></IconCell>
						<IconCell label="Camera"><IconCamera size={SIZE} /></IconCell>
						<IconCell label="ChevronRight"><IconChevronRight size={SIZE} /></IconCell>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Instagram"><IconBrandInstagram size={SIZE} /></IconCell>
						<IconCell label="WhatsApp"><IconBrandWhatsapp size={SIZE} /></IconCell>
						<IconCell label="Github"><IconBrandGithub size={SIZE} /></IconCell>
						<IconCell label="Twitter/X"><IconBrandTwitter size={SIZE} /></IconCell>
						<IconCell label="TikTok"><IconBrandTiktok size={SIZE} /></IconCell>
					</div>
				</div>
			</section>

			<!-- PHOSPHOR -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8">
				<div class="mb-6 flex flex-wrap items-baseline gap-x-6 gap-y-2">
					<h2 class="text-2xl font-semibold text-white">phosphor-svelte</h2>
					<span class="rounded-full bg-violet-500/10 px-3 py-0.5 text-sm text-violet-400">v3.1.0</span>
				</div>

				<div class="mb-6 grid grid-cols-2 gap-4 text-sm text-zinc-400 sm:grid-cols-4">
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Icons</span>
						<span class="text-zinc-200">~1,500+ (6 weights)</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Brand Icons</span>
						<span class="text-emerald-400">Yes</span>
						<span class="block text-xs text-zinc-500">Instagram, WhatsApp, Github, X, TikTok</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Tree-shakeable</span>
						<span class="text-emerald-400">Yes</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Bundle per icon</span>
						<span class="text-zinc-200">~1 KB</span>
					</div>
				</div>

				<div class="mb-4">
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Common Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="House"><PhosphorHouse size={SIZE} /></IconCell>
						<IconCell label="Search"><PhosphorSearch size={SIZE} /></IconCell>
						<IconCell label="Gear"><PhosphorGear size={SIZE} /></IconCell>
						<IconCell label="Heart"><PhosphorHeart size={SIZE} /></IconCell>
						<IconCell label="Star"><PhosphorStar size={SIZE} /></IconCell>
						<IconCell label="Calendar"><PhosphorCalendar size={SIZE} /></IconCell>
						<IconCell label="Envelope"><PhosphorEnvelope size={SIZE} /></IconCell>
						<IconCell label="Phone"><PhosphorPhone size={SIZE} /></IconCell>
						<IconCell label="Camera"><PhosphorCamera size={SIZE} /></IconCell>
						<IconCell label="CaretRight"><PhosphorCaretRight size={SIZE} /></IconCell>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Instagram"><PhosphorInstagram size={SIZE} /></IconCell>
						<IconCell label="WhatsApp"><PhosphorWhatsapp size={SIZE} /></IconCell>
						<IconCell label="Github"><PhosphorGithub size={SIZE} /></IconCell>
						<IconCell label="X (Twitter)"><PhosphorX size={SIZE} /></IconCell>
						<IconCell label="TikTok"><PhosphorTiktok size={SIZE} /></IconCell>
					</div>
				</div>
			</section>

			<!-- REMIX -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8">
				<div class="mb-6 flex flex-wrap items-baseline gap-x-6 gap-y-2">
					<h2 class="text-2xl font-semibold text-white">svelte-remix</h2>
					<span class="rounded-full bg-orange-500/10 px-3 py-0.5 text-sm text-orange-400">v3.0.1</span>
				</div>

				<div class="mb-6 grid grid-cols-2 gap-4 text-sm text-zinc-400 sm:grid-cols-4">
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Icons</span>
						<span class="text-zinc-200">~2,800+ (fill + line)</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Brand Icons</span>
						<span class="text-emerald-400">Yes</span>
						<span class="block text-xs text-zinc-500">Instagram, WhatsApp, Github, Twitter, TikTok</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Tree-shakeable</span>
						<span class="text-emerald-400">Yes</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Bundle per icon</span>
						<span class="text-zinc-200">~1 KB</span>
					</div>
				</div>

				<div class="mb-4">
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Common Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Home"><RemixHome size={`${SIZE}`} /></IconCell>
						<IconCell label="Search"><RemixSearch size={`${SIZE}`} /></IconCell>
						<IconCell label="Settings"><RemixSettings size={`${SIZE}`} /></IconCell>
						<IconCell label="Heart"><RemixHeart size={`${SIZE}`} /></IconCell>
						<IconCell label="Star"><RemixStar size={`${SIZE}`} /></IconCell>
						<IconCell label="Calendar"><RemixCalendar size={`${SIZE}`} /></IconCell>
						<IconCell label="Mail"><RemixMail size={`${SIZE}`} /></IconCell>
						<IconCell label="Phone"><RemixPhone size={`${SIZE}`} /></IconCell>
						<IconCell label="Camera"><RemixCamera size={`${SIZE}`} /></IconCell>
						<IconCell label="ChevronRight"><RemixChevronRight size={`${SIZE}`} /></IconCell>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Instagram"><RemixInstagram size={`${SIZE}`} /></IconCell>
						<IconCell label="WhatsApp"><RemixWhatsapp size={`${SIZE}`} /></IconCell>
						<IconCell label="Github"><RemixGithub size={`${SIZE}`} /></IconCell>
						<IconCell label="Twitter/X"><RemixTwitter size={`${SIZE}`} /></IconCell>
						<IconCell label="TikTok"><RemixTiktok size={`${SIZE}`} /></IconCell>
					</div>
				</div>
			</section>

			<!-- HUGEICONS -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8">
				<div class="mb-6 flex flex-wrap items-baseline gap-x-6 gap-y-2">
					<h2 class="text-2xl font-semibold text-white">@hugeicons/svelte</h2>
					<span class="rounded-full bg-pink-500/10 px-3 py-0.5 text-sm text-pink-400">v1.1.2</span>
				</div>

				<div class="mb-6 grid grid-cols-2 gap-4 text-sm text-zinc-400 sm:grid-cols-4">
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Icons</span>
						<span class="text-zinc-200">5,100+ free (51k pro)</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Brand Icons</span>
						<span class="text-emerald-400">Yes</span>
						<span class="block text-xs text-zinc-500">Instagram, WhatsApp, Github, Twitter, TikTok</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Tree-shakeable</span>
						<span class="text-emerald-400">Yes</span>
					</div>
					<div>
						<span class="block text-xs uppercase tracking-wider text-zinc-500">Bundle per icon</span>
						<span class="text-zinc-200">~1 KB (data object)</span>
					</div>
				</div>

				<div class="mb-4">
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Common Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Home"><HugeiconsIcon icon={Home01Icon} size={SIZE} /></IconCell>
						<IconCell label="Search"><HugeiconsIcon icon={Search01Icon} size={SIZE} /></IconCell>
						<IconCell label="Settings"><HugeiconsIcon icon={Settings01Icon} size={SIZE} /></IconCell>
						<IconCell label="Heart"><HugeiconsIcon icon={FavouriteIcon} size={SIZE} /></IconCell>
						<IconCell label="Star"><HugeiconsIcon icon={StarIcon} size={SIZE} /></IconCell>
						<IconCell label="Calendar"><HugeiconsIcon icon={Calendar01Icon} size={SIZE} /></IconCell>
						<IconCell label="Mail"><HugeiconsIcon icon={Mail01Icon} size={SIZE} /></IconCell>
						<IconCell label="Phone"><HugeiconsIcon icon={TelephoneIcon} size={SIZE} /></IconCell>
						<IconCell label="Camera"><HugeiconsIcon icon={Camera01Icon} size={SIZE} /></IconCell>
						<IconCell label="ArrowRight"><HugeiconsIcon icon={ArrowRight01Icon} size={SIZE} /></IconCell>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<IconCell label="Instagram"><HugeiconsIcon icon={InstagramIcon} size={SIZE} /></IconCell>
						<IconCell label="WhatsApp"><HugeiconsIcon icon={WhatsappIcon} size={SIZE} /></IconCell>
						<IconCell label="Github"><HugeiconsIcon icon={GithubIcon} size={SIZE} /></IconCell>
						<IconCell label="Twitter/X"><HugeiconsIcon icon={TwitterIcon} size={SIZE} /></IconCell>
						<IconCell label="TikTok"><HugeiconsIcon icon={TiktokIcon} size={SIZE} /></IconCell>
					</div>
				</div>
			</section>
		</div>

		<!-- Summary Table -->
		<div class="mt-16 overflow-x-auto rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8">
			<h2 class="mb-6 text-2xl font-semibold text-white">Quick Comparison</h2>
			<table class="w-full text-left text-sm">
				<thead>
					<tr class="border-b border-zinc-800 text-xs uppercase tracking-wider text-zinc-500">
						<th class="pb-3 pr-6">Library</th>
						<th class="pb-3 pr-6">Icons</th>
						<th class="pb-3 pr-6">Brand Icons</th>
						<th class="pb-3 pr-6">Tree-shake</th>
						<th class="pb-3 pr-6">Import Pattern</th>
						<th class="pb-3">Notes</th>
					</tr>
				</thead>
				<tbody class="text-zinc-300">
					<tr class="border-b border-zinc-800/50">
						<td class="py-3 pr-6 font-medium text-white">@lucide/svelte</td>
						<td class="py-3 pr-6">~1,500+</td>
						<td class="py-3 pr-6 text-red-400">No</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6"><code class="rounded bg-zinc-800 px-1.5 py-0.5 text-xs">Home</code></td>
						<td class="py-3">Clean, minimal. Brand icons removed in v1.x.</td>
					</tr>
					<tr class="border-b border-zinc-800/50">
						<td class="py-3 pr-6 font-medium text-white">@tabler/icons-svelte</td>
						<td class="py-3 pr-6">~5,800+</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6"><code class="rounded bg-zinc-800 px-1.5 py-0.5 text-xs">IconHome</code></td>
						<td class="py-3">Largest free set. Full brand coverage. 2px stroke default.</td>
					</tr>
					<tr class="border-b border-zinc-800/50">
						<td class="py-3 pr-6 font-medium text-white">phosphor-svelte</td>
						<td class="py-3 pr-6">~1,500+ (6w)</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6"><code class="rounded bg-zinc-800 px-1.5 py-0.5 text-xs">House</code></td>
						<td class="py-3">6 weight variants per icon. Unique naming (House, Envelope, Gear).</td>
					</tr>
					<tr class="border-b border-zinc-800/50">
						<td class="py-3 pr-6 font-medium text-white">svelte-remix</td>
						<td class="py-3 pr-6">~2,800+</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6"><code class="rounded bg-zinc-800 px-1.5 py-0.5 text-xs">HomeLineBuildings</code></td>
						<td class="py-3">Verbose naming with category suffix. Fill + Line variants.</td>
					</tr>
					<tr>
						<td class="py-3 pr-6 font-medium text-white">@hugeicons/svelte</td>
						<td class="py-3 pr-6">5,100+ (51k pro)</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6 text-emerald-400">Yes</td>
						<td class="py-3 pr-6"><code class="rounded bg-zinc-800 px-1.5 py-0.5 text-xs">Home01Icon</code></td>
						<td class="py-3">Data-driven (icon prop). Needs separate @hugeicons/core-free-icons package.</td>
					</tr>
				</tbody>
			</table>
		</div>

		<footer class="mt-12 text-center text-sm text-zinc-600">
			Generated for Studio Petite icon library evaluation
		</footer>
	</div>
</div>
