<script>
	import { Section, HeroHeader, FeatureDefault, FeatureItem } from 'flowbite-svelte-blocks';
	import {
		Button,
		Navbar,
		NavBrand,
		NavHamburger,
		NavUl,
		NavLi,
		Img,
		Heading,
		P,
		A,
		Footer,
		FooterCopyright,
		FooterLinkGroup,
		FooterLink
	} from 'flowbite-svelte';
	import {
		ArrowRightOutline,
		RectangleListOutline,
		SearchOutline,
		SunOutline,
		TextSizeOutline,
		ForwardOutline,
		GlobeOutline
	} from 'flowbite-svelte-icons';
	import favicon from '$lib/assets/favicon.svg';
</script>

<svelte:head>
	<title>Gearence</title>
</svelte:head>

<Navbar>
	<NavBrand href="/">
		<img src={favicon} class="me-3 h-6 sm:h-9" alt="Flowbite Logo" />
		<span class="self-center text-xl font-semibold whitespace-nowrap dark:text-white">Gearence</span
		>
	</NavBrand>
	<NavHamburger />
	<NavUl>
		<NavLi href="/">Home</NavLi>
		<NavLi href="#download">Download</NavLi>
		<NavLi href="#feature">Features</NavLi>
		<NavLi href="#contact">Contact</NavLi>
	</NavUl>
</Navbar>

<Section name="heroVisual">
	<div class="mr-auto place-self-center lg:col-span-7">
		<HeroHeader
			h1Class="max-w-2xl mb-4 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white"
			pClass="text-left max-w-2xl mb-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400 sm:px-0 lg:px-0 xl:px-0"
		>
			{#snippet h1()}
				The Ultimate Offline Godot Class Reference.
			{/snippet}
			{#snippet paragraph()}High-performance documentation for every major Godot version, right in
				your pocket. Covering version 2.0 to 4.6.
			{/snippet}
			<a href="#download"
				><Button size="xl" class="mr-3 inline-flex items-center justify-center"
					>Download<ArrowRightOutline size="md" class="-mr-1 ml-2" /></Button
				>
			</a>
		</HeroHeader>
	</div>
	<div class="hidden lg:col-span-5 lg:mt-0 lg:flex">
		<img src={favicon} alt="mockup" />
	</div>
</Section>

<Section>
	<div class="grid grid-cols-1 md:grid-cols-2" id="download">
		<Img
			src="/appstore-badge.png"
			href="https://apps.apple.com/qa/app/godot-class-reference/id1523486419"
		/>
		<Img
			src="/google-play-badge.png"
			href="https://play.google.com/store/apps/details?id=com.fengjiongmax.godotclassreference"
		/>
	</div>
</Section>

<Section name="feature">
	<div id="feature">
		<HeroHeader
			class="mb-8 max-w-3xl lg:mb-16"
			h2Class="mb-4 lg:mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white text-left"
			pClass="text-gray-500 sm:text-xl dark:text-gray-400 text-left sm:px-0 xl:px-0"
		>
			{#snippet h2()}Fast. Offline. Version-Versatile{/snippet}
			{#snippet paragraph()}Access the complete Godot Class Reference anywhere. Featuring instant
				search, native system theming, and localized content for a distraction-free coding
				experience.{/snippet}
		</HeroHeader>

		<FeatureDefault>
			<FeatureItem>
				{#snippet icon()}
					<RectangleListOutline class="text-primary-600 dark:text-primary-300" />
				{/snippet}
				{#snippet h3()}
					Multiple Versions.
				{/snippet}
				{#snippet paragraph()}
					Comprehensive documentation support for Godot 2.0 through the latest 4.x releases.
				{/snippet}
			</FeatureItem>
			<FeatureItem>
				{#snippet icon()}
					<SearchOutline class="text-primary-600 dark:text-primary-300" />
				{/snippet}
				{#snippet h3()}
					Instant Search
				{/snippet}
				{#snippet paragraph()}
					Effortless navigation with optimized in-app search functionality.
				{/snippet}
			</FeatureItem>
			<FeatureItem>
				{#snippet icon()}
					<ForwardOutline class="text-primary-600 dark:text-primary-300" />
				{/snippet}
				{#snippet h3()}
					In-app Redirection
				{/snippet}
				{#snippet paragraph()}
					Seamlessly jump between classes, functions, signals, and properties with intuitive
					deep-linking.
				{/snippet}
			</FeatureItem>
			<FeatureItem>
				{#snippet icon()}
					<SunOutline class="text-primary-600 dark:text-primary-300" />
				{/snippet}
				{#snippet h3()}
					Native Dark Mode
				{/snippet}
				{#snippet paragraph()}
					Enjoy a comfortable reading experience with a UI that adapts instantly to your system
					theme.
				{/snippet}
			</FeatureItem>
			<FeatureItem>
				{#snippet icon()}
					<TextSizeOutline class="text-primary-600 dark:text-primary-300" />
				{/snippet}
				{#snippet h3()}
					Adjustable Typography
				{/snippet}
				{#snippet paragraph()}
					Customize your reading experience with adjustable text sizes and high-quality mono fonts.
				{/snippet}
			</FeatureItem>
			<FeatureItem>
				{#snippet icon()}
					<GlobeOutline class="text-primary-600 dark:text-primary-300" />
				{/snippet}
				{#snippet h3()}
					Offline First
				{/snippet}
				{#snippet paragraph()}
					All data is stored locally in a high-performance database, ensuring documentation is
					available whenever you are.
				{/snippet}
			</FeatureItem>
		</FeatureDefault>
	</div>
</Section>

<Section>
	<div id="contact">
		<Heading>Contact</Heading>
		<br />
		<P
			>If you have encountered any problem,sent an email to <A
				href="mailto:fengjiongmax+gearence@gmail.com">fengjiongmax+gearence@gmail.com</A
			>.</P
		>
	</div>
</Section>

<Section>
	<div id="privacy_policy">
		<Heading>Privacy Policy</Heading>
		<br />
		<P>Gearence does not collect any user data.</P>
	</div>
</Section>

<Footer>
	<FooterCopyright href="/" by="Gearence" year={2026} />
	<FooterLinkGroup
		class="mt-3 flex flex-wrap items-center text-sm text-gray-500 sm:mt-0 dark:text-gray-400"
	>
		<FooterLink href="#privacy_policy">Privacy Policy</FooterLink>

		<FooterLink href="https://github.com/GodotDocMobile/godot_class_reference"
			>Source Code</FooterLink
		>
	</FooterLinkGroup>
</Footer>
