<script lang="ts">
	// Lucide (v0.561.0)
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

	// Tabler (v3.41.1)
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

	// Phosphor (v3.1.0)
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

	// Remix (v3.0.1) — uses CategorySuffix naming convention
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

	// Hugeicons (v1.1.2) — uses HugeiconsIcon component + icon data objects
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

	const SIZE = 24;
	const REMIX_SIZE = `${SIZE}`;
</script>

<svelte:head>
	<title>Icon Library Comparison</title>
</svelte:head>

<div class="min-h-screen bg-zinc-950 text-zinc-100 px-6 py-12 font-sans">
	<div class="mx-auto max-w-7xl">
		<!-- Header -->
		<header class="mb-16 text-center">
			<h1 class="text-4xl font-bold tracking-tight text-white sm:text-5xl">
				Svelte Icon Libraries
			</h1>
			<p class="mt-4 text-lg text-zinc-400">
				Side-by-side comparison of 5 popular icon packages for Svelte 5
			</p>
		</header>

		<!-- Grid of Cards -->
		<div class="grid gap-8">

			<!-- ======================== LUCIDE ======================== -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8 backdrop-blur">
				<div class="mb-6 flex flex-wrap items-baseline gap-x-6 gap-y-2">
					<h2 class="text-2xl font-semibold text-white">@lucide/svelte</h2>
					<span class="rounded-full bg-emerald-500/10 px-3 py-0.5 text-sm text-emerald-400">v0.561.0</span>
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
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideHome size={SIZE} /></div><span class="text-[10px] text-zinc-500">Home</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideSearch size={SIZE} /></div><span class="text-[10px] text-zinc-500">Search</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideSettings size={SIZE} /></div><span class="text-[10px] text-zinc-500">Settings</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideHeart size={SIZE} /></div><span class="text-[10px] text-zinc-500">Heart</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideStar size={SIZE} /></div><span class="text-[10px] text-zinc-500">Star</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideCalendar size={SIZE} /></div><span class="text-[10px] text-zinc-500">Calendar</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideMail size={SIZE} /></div><span class="text-[10px] text-zinc-500">Mail</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucidePhone size={SIZE} /></div><span class="text-[10px] text-zinc-500">Phone</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideCamera size={SIZE} /></div><span class="text-[10px] text-zinc-500">Camera</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><LucideChevronRight size={SIZE} /></div><span class="text-[10px] text-zinc-500">ChevronRight</span></div>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/40 text-zinc-600"><span class="text-xs">N/A</span></div><span class="text-[10px] text-zinc-500">Instagram</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/40 text-zinc-600"><span class="text-xs">N/A</span></div><span class="text-[10px] text-zinc-500">WhatsApp</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/40 text-zinc-600"><span class="text-xs">N/A</span></div><span class="text-[10px] text-zinc-500">Github</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/40 text-zinc-600"><span class="text-xs">N/A</span></div><span class="text-[10px] text-zinc-500">Twitter/X</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/40 text-zinc-600"><span class="text-xs">N/A</span></div><span class="text-[10px] text-zinc-500">TikTok</span></div>
					</div>
				</div>
			</section>

			<!-- ======================== TABLER ======================== -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8 backdrop-blur">
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
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconHome size={SIZE} /></div><span class="text-[10px] text-zinc-500">Home</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconSearch size={SIZE} /></div><span class="text-[10px] text-zinc-500">Search</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconSettings size={SIZE} /></div><span class="text-[10px] text-zinc-500">Settings</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconHeart size={SIZE} /></div><span class="text-[10px] text-zinc-500">Heart</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconStar size={SIZE} /></div><span class="text-[10px] text-zinc-500">Star</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconCalendar size={SIZE} /></div><span class="text-[10px] text-zinc-500">Calendar</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconMail size={SIZE} /></div><span class="text-[10px] text-zinc-500">Mail</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconPhone size={SIZE} /></div><span class="text-[10px] text-zinc-500">Phone</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconCamera size={SIZE} /></div><span class="text-[10px] text-zinc-500">Camera</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconChevronRight size={SIZE} /></div><span class="text-[10px] text-zinc-500">ChevronRight</span></div>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconBrandInstagram size={SIZE} /></div><span class="text-[10px] text-zinc-500">Instagram</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconBrandWhatsapp size={SIZE} /></div><span class="text-[10px] text-zinc-500">WhatsApp</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconBrandGithub size={SIZE} /></div><span class="text-[10px] text-zinc-500">Github</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconBrandTwitter size={SIZE} /></div><span class="text-[10px] text-zinc-500">Twitter/X</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><IconBrandTiktok size={SIZE} /></div><span class="text-[10px] text-zinc-500">TikTok</span></div>
					</div>
				</div>
			</section>

			<!-- ======================== PHOSPHOR ======================== -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8 backdrop-blur">
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
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorHouse size={SIZE} /></div><span class="text-[10px] text-zinc-500">House</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorSearch size={SIZE} /></div><span class="text-[10px] text-zinc-500">Search</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorGear size={SIZE} /></div><span class="text-[10px] text-zinc-500">Gear</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorHeart size={SIZE} /></div><span class="text-[10px] text-zinc-500">Heart</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorStar size={SIZE} /></div><span class="text-[10px] text-zinc-500">Star</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorCalendar size={SIZE} /></div><span class="text-[10px] text-zinc-500">Calendar</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorEnvelope size={SIZE} /></div><span class="text-[10px] text-zinc-500">Envelope</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorPhone size={SIZE} /></div><span class="text-[10px] text-zinc-500">Phone</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorCamera size={SIZE} /></div><span class="text-[10px] text-zinc-500">Camera</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorCaretRight size={SIZE} /></div><span class="text-[10px] text-zinc-500">CaretRight</span></div>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorInstagram size={SIZE} /></div><span class="text-[10px] text-zinc-500">Instagram</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorWhatsapp size={SIZE} /></div><span class="text-[10px] text-zinc-500">WhatsApp</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorGithub size={SIZE} /></div><span class="text-[10px] text-zinc-500">Github</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorX size={SIZE} /></div><span class="text-[10px] text-zinc-500">X (Twitter)</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><PhosphorTiktok size={SIZE} /></div><span class="text-[10px] text-zinc-500">TikTok</span></div>
					</div>
				</div>
			</section>

			<!-- ======================== REMIX ======================== -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8 backdrop-blur">
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
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixHome size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Home</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixSearch size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Search</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixSettings size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Settings</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixHeart size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Heart</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixStar size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Star</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixCalendar size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Calendar</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixMail size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Mail</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixPhone size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Phone</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixCamera size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Camera</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixChevronRight size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">ChevronRight</span></div>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixInstagram size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Instagram</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixWhatsapp size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">WhatsApp</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixGithub size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Github</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixTwitter size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">Twitter/X</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><RemixTiktok size={REMIX_SIZE} /></div><span class="text-[10px] text-zinc-500">TikTok</span></div>
					</div>
				</div>
			</section>

			<!-- ======================== HUGEICONS ======================== -->
			<section class="rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8 backdrop-blur">
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
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={Home01Icon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Home</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={Search01Icon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Search</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={Settings01Icon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Settings</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={FavouriteIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Heart</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={StarIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Star</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={Calendar01Icon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Calendar</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={Mail01Icon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Mail</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={TelephoneIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Phone</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={Camera01Icon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Camera</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={ArrowRight01Icon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">ArrowRight</span></div>
					</div>
				</div>

				<div>
					<h3 class="mb-3 text-xs uppercase tracking-wider text-zinc-500">Brand Icons</h3>
					<div class="flex flex-wrap gap-6">
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={InstagramIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Instagram</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={WhatsappIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">WhatsApp</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={GithubIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Github</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={TwitterIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">Twitter/X</span></div>
						<div class="flex flex-col items-center gap-1.5"><div class="flex h-12 w-12 items-center justify-center rounded-xl bg-zinc-800/80 transition-colors hover:bg-zinc-700/80"><HugeiconsIcon icon={TiktokIcon} size={SIZE} /></div><span class="text-[10px] text-zinc-500">TikTok</span></div>
					</div>
				</div>
			</section>
		</div>

		<!-- Summary Table -->
		<div class="mt-16 overflow-x-auto rounded-2xl border border-zinc-800 bg-zinc-900/60 p-8 backdrop-blur">
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
