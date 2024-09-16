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
		BriefcaseSolid,
		SunOutline,
		TextSizeOutline,
		ForwardOutline,
		CogOutline
	} from 'flowbite-svelte-icons';
</script>

<svelte:head>
	<title>Gearence</title>
</svelte:head>

<Navbar>
	<NavBrand href="/">
		<!-- <img src="/images/flowbite-svelte-icon-logo.svg" class="me-3 h-6 sm:h-9" alt="Flowbite Logo" /> -->
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Gearence</span
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
			pClass="max-w-2xl mb-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400"
		>
			<svelte:fragment slot="h1">Third party Godot Class Reference reader.</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Gearence contains class documentation covering version 2.0 to 4.3.</svelte:fragment
			>
			<a href="#download"
				><Button size="xl" class="mr-3 inline-flex items-center justify-center"
					>Download<ArrowRightOutline size="md" class="-mr-1 ml-2" /></Button
				>
			</a>
			<!-- <a href="/"
				><Button color="light" size="xl" class="inline-flex items-center justify-center"
					>Speak to Sales</Button
				>
			</a> -->
		</HeroHeader>
	</div>
	<div class="hidden lg:col-span-5 lg:mt-0 lg:flex">
		<img src="/icon_transparent.png" alt="mockup" />
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
			class="mb-8 max-w-screen-md lg:mb-16"
			h2Class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white"
			pClass="text-gray-500 sm:text-xl dark:text-gray-400"
		>
			<svelte:fragment slot="h2">Gearence</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Embark on your journey through the world of Godot Engine with unparalleled convenience.</svelte:fragment
			>
		</HeroHeader>
		<FeatureDefault>
			<FeatureItem>
				<svelte:fragment slot="icon"
					><RectangleListOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
				>
				<svelte:fragment slot="h3">Multiple Versions.</svelte:fragment>
				<svelte:fragment slot="paragraph"
					>Comprehensive documentation for multiple Godot versions.</svelte:fragment
				>
			</FeatureItem>
			<FeatureItem>
				<svelte:fragment slot="icon"
					><SearchOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
				>
				<svelte:fragment slot="h3">In-app Search</svelte:fragment>
				<svelte:fragment slot="paragraph"
					>Effortless navigation with in-app search functionality.</svelte:fragment
				>
			</FeatureItem>
			<FeatureItem>
				<svelte:fragment slot="icon"
					><ForwardOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
				>
				<svelte:fragment slot="h3">In-app Redirection</svelte:fragment>
				<svelte:fragment slot="paragraph"
					>Seamlessly switch between classes, functions, signals, and properties with in-app
					redirection.</svelte:fragment
				>
			</FeatureItem>
			<FeatureItem>
				<svelte:fragment slot="icon"
					><SunOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
				>
				<svelte:fragment slot="h3">Dark Mode</svelte:fragment>
				<svelte:fragment slot="paragraph">Enjoy comfortable reading with Dark Mode.</svelte:fragment
				>
			</FeatureItem>
			<FeatureItem>
				<svelte:fragment slot="icon"
					><TextSizeOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
				>
				<svelte:fragment slot="h3">Adjustable text size</svelte:fragment>
				<svelte:fragment slot="paragraph"
					>Customize your reading experience with adjustable text size.</svelte:fragment
				>
			</FeatureItem>
			<!-- <FeatureItem>
				<svelte:fragment slot="icon"
					><CogOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
				>
				<svelte:fragment slot="h3">Operations</svelte:fragment>
				<svelte:fragment slot="paragraph"
					>Keep your company’s lights on with customizable, iterative, and structured workflows
					built for all efficient teams and individual.</svelte:fragment
				>
			</FeatureItem> -->
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

<Section>
	<Footer>
		<div class="sm:flex sm:items-center sm:justify-between">
			<FooterCopyright href="/" by="Gearence" year={2024} />
			<FooterLinkGroup
				ulClass="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0"
			>
				<!-- <FooterLink href="/">About</FooterLink> -->
				<FooterLink href="#privacy_policy">Privacy Policy</FooterLink>
				<FooterLink href="https://github.com/GodotDocMobile/godot_class_reference"
					>Source Code</FooterLink
				>
			</FooterLinkGroup>
		</div>
	</Footer>
</Section>
