<script lang="ts">
	// Icons
	const icons = {
		logo: `<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-6 h-6"><path fill-rule="evenodd" clip-rule="evenodd" d="M6.99251 12.196C6.85314 12.5757 6.62925 12.9208 6.33682 13.2067H6.33835C6.00191 13.5351 5.58566 13.7756 5.12816 13.9059C4.67065 14.0362 4.18671 14.0522 3.72118 13.9523C3.25564 13.8524 2.82357 13.64 2.46501 13.3345C2.10645 13.0291 1.83299 12.6406 1.66998 12.2051C1.50697 11.7696 1.45969 11.3012 1.5325 10.8432C1.60532 10.3852 1.79587 9.95244 2.08653 9.58516C2.37718 9.21781 2.75852 8.9277 3.1952 8.74177C3.63188 8.55585 4.10979 8.48002 4.58462 8.52142L4.57074 8.50792C5.0567 8.54782 5.54575 8.48407 6.00378 8.32124C6.4618 8.15846 6.87776 7.90043 7.2226 7.56521C7.56746 7.22998 7.83285 6.82564 8.00036 6.38041C8.16786 5.93517 8.23344 5.45976 8.1924 4.98737L8.20628 5.00087C8.15181 4.43594 8.27796 3.86844 8.56753 3.37575C8.85701 2.88307 9.29579 2.48919 9.82407 2.24782C10.3523 2.00645 10.9443 1.92933 11.5192 2.02701C12.0942 2.12467 12.6243 2.39237 13.037 2.79358C13.4497 3.19479 13.7251 3.70999 13.8256 4.26892C13.926 4.82785 13.8467 5.4033 13.5984 5.9168C13.3501 6.4303 12.9449 6.85685 12.4381 7.13828C11.9313 7.41971 11.3474 7.54233 10.7663 7.4894L10.781 7.5029C10.2949 7.46279 9.80563 7.52632 9.34741 7.68904C8.88919 7.85176 8.47309 8.10975 8.12805 8.44499C7.78301 8.78025 7.51742 9.18466 7.34983 9.63001C7.18224 10.0754 7.11669 10.551 7.15774 11.0235L7.14309 11.01C7.1833 11.4112 7.13189 11.8162 6.99251 12.196ZM11.5077 14.7121L11.493 14.6986C11.9061 14.739 12.3232 14.6897 12.7143 14.5543C13.1053 14.4188 13.4605 14.2007 13.7542 13.9154C14.0477 13.6302 14.2726 13.285 14.4121 12.905C14.5518 12.525 14.6028 12.1196 14.5615 11.718L14.5762 11.7315C14.5351 11.2591 14.6007 10.7838 14.7681 10.3385C14.9356 9.89327 15.2011 9.48893 15.5459 9.15368C15.8908 8.8185 16.3068 8.56042 16.7648 8.39767C17.2228 8.23481 17.7118 8.17111 18.1978 8.21099L18.1832 8.19749C18.7645 8.25059 19.3485 8.12801 19.8556 7.84656C20.3627 7.56511 20.7681 7.13845 21.0165 6.62479C21.265 6.11114 21.3444 5.53548 21.2439 4.97634C21.1435 4.4172 20.868 3.9018 20.4551 3.50044C20.0422 3.09909 19.512 2.8313 18.9368 2.73364C18.3616 2.63596 17.7695 2.71315 17.241 2.95467C16.7126 3.19618 16.2737 3.59027 15.9842 4.08319C15.6946 4.57609 15.5685 5.14383 15.6232 5.70895L15.6093 5.6947C15.6504 6.16712 15.585 6.64259 15.4175 7.08788C15.2501 7.53318 14.9846 7.93758 14.6398 8.27287C14.2949 8.60805 13.8789 8.86612 13.4208 9.02888C12.9627 9.19163 12.4736 9.25523 11.9876 9.21526L12.0015 9.22951C11.5885 9.18908 11.1713 9.23836 10.7803 9.37381C10.3893 9.50919 10.034 9.72744 9.74039 10.0127C9.44674 10.2979 9.22199 10.6431 9.08234 11.0231C8.94276 11.4031 8.89176 11.8085 8.93304 12.2101L8.91915 12.1966C8.96005 12.6689 8.89439 13.1443 8.72688 13.5895C8.5593 14.0346 8.29389 14.4389 7.94908 14.7741C7.60425 15.1093 7.18835 15.3673 6.73039 15.5302C6.27242 15.693 5.78342 15.7569 5.29749 15.7171L5.31138 15.7306C4.73003 15.6775 4.14599 15.8001 3.63892 16.0815C3.13186 16.363 2.72644 16.7896 2.478 17.3033C2.22954 17.817 2.15013 18.3926 2.25061 18.9518C2.35109 19.5109 2.62657 20.0263 3.03945 20.4276C3.45234 20.829 3.98253 21.0968 4.55773 21.1944C5.13293 21.2921 5.72512 21.2149 6.25353 20.9734C6.78193 20.7319 7.22085 20.3379 7.51038 19.8449C7.79994 19.352 7.92601 18.7843 7.87139 18.2191L7.88605 18.2326C7.845 17.7602 7.91058 17.2849 8.07809 16.8396C8.24551 16.3944 8.511 15.99 8.85581 15.6548C9.20069 15.3196 9.61664 15.0615 10.0746 14.8988C10.5327 14.7359 11.0217 14.6722 11.5077 14.7121ZM17.1996 10.7633C16.9071 11.0493 16.6832 11.3944 16.5437 11.7741C16.4042 12.1538 16.3526 12.5587 16.3925 12.9601L16.3786 12.9466C16.4197 13.419 16.3541 13.8944 16.1866 14.3396C16.0191 14.7849 15.7537 15.1892 15.4089 15.5244C15.064 15.8596 14.648 16.1177 14.19 16.2804C13.732 16.4433 13.2429 16.507 12.757 16.4671L12.7708 16.4806C12.1896 16.4281 11.6057 16.551 11.0989 16.8328C10.5921 17.1145 10.1871 17.5414 9.93902 18.0551C9.69097 18.5689 9.61188 19.1444 9.71265 19.7035C9.81349 20.2625 10.0892 20.7777 10.5022 21.1788C10.9152 21.5799 11.4454 21.8474 12.0205 21.9448C12.5957 22.0423 13.1877 21.9649 13.716 21.7234C14.2443 21.4817 14.683 21.0877 14.9724 20.5947C15.2618 20.1018 15.3878 19.5342 15.3332 18.9692L15.3478 18.9827C15.3068 18.5103 15.3723 18.0349 15.5398 17.5896C15.7073 17.1444 15.9728 16.7401 16.3176 16.4048C16.6625 16.0696 17.0784 15.8115 17.5364 15.6488C17.9945 15.486 18.4835 15.4222 18.9695 15.4621L18.9548 15.4486C19.4296 15.4901 19.9076 15.4144 20.3444 15.2286C20.7811 15.0427 21.1625 14.7527 21.4533 14.3854C21.744 14.0181 21.9347 13.5854 22.0075 13.1274C22.0805 12.6694 22.0332 12.2009 21.8703 11.7653C21.7073 11.3298 21.4339 10.9413 21.0754 10.6358C20.7168 10.3303 20.2848 10.1178 19.8192 10.0179C19.3536 9.91795 18.8697 9.93385 18.4121 10.0641C17.9546 10.1945 17.5383 10.4349 17.2019 10.7633H17.1996Z" fill="currentColor"/></svg>`,
		clock: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>`,
		arrowRight: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><line x1="5" y1="12" x2="19" y2="12"/><polyline points="12 5 19 12 12 19"/></svg>`,
		reflection: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>`,
		productivity: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"/></svg>`,
		memory: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M9.5 2A2.5 2.5 0 0 1 12 4.5v15a2.5 2.5 0 0 1-4.96.44 2.5 2.5 0 0 1-2.96-3.08 3 3 0 0 1-.34-5.58 2.5 2.5 0 0 1 1.32-4.24 2.5 2.5 0 0 1 1.98-3A2.5 2.5 0 0 1 9.5 2Z"/><path d="M14.5 2A2.5 2.5 0 0 0 12 4.5v15a2.5 2.5 0 0 0 4.96.44 2.5 2.5 0 0 0 2.96-3.08 3 3 0 0 0 .34-5.58 2.5 2.5 0 0 0-1.32-4.24 2.5 2.5 0 0 0-1.98-3A2.5 2.5 0 0 0 14.5 2Z"/></svg>`,
		clarity: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M12 2v4"/><path d="M12 18v4"/><path d="M4.93 4.93l2.83 2.83"/><path d="M16.24 16.24l2.83 2.83"/><path d="M2 12h4"/><path d="M18 12h4"/><path d="M4.93 19.07l2.83-2.83"/><path d="M16.24 7.76l2.83-2.83"/></svg>`,
		speedometer: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5"><path d="M22 12A10 10 0 0 0 12 2v10z"/></svg>`, // Simplified
		shield: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>`,
		sparkles: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5"><path d="m12 3-1.912 5.813a2 2 0 0 1-1.275 1.275L3 12l5.813 1.912a2 2 0 0 1 1.275 1.275L12 21l1.912-5.813a2 2 0 0 1 1.275-1.275L21 12l-5.813-1.912a2 2 0 0 1-1.275-1.275L12 3Z"/></svg>`,
		soundwave: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5"><path d="M12 2v20"/><path d="M16 6v12"/><path d="M20 10v4"/><path d="M8 6v12"/><path d="M4 10v4"/></svg>`,
		plus: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>`,
		check: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><polyline points="20 6 9 17 4 12"/></svg>`,
		calendar: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>`,
		repeat: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><polyline points="17 1 21 5 17 9"/><path d="M3 11V9a4 4 0 0 1 4-4h14"/><polyline points="7 23 3 19 7 15"/><path d="M21 13v2a4 4 0 0 1-4 4H3"/></svg>`,
		search: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><circle cx="11" cy="11" r="8"/><line x1="21" y1="21" x2="16.65" y2="16.65"/></svg>`,
		camera: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"/><circle cx="12" cy="13" r="4"/></svg>`,
		mic: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" y1="19" x2="12" y2="23"/><line x1="8" y1="23" x2="16" y2="23"/></svg>`,
		download: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>`,
		layout: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"/><line x1="3" y1="9" x2="21" y2="9"/><line x1="9" y1="21" x2="9" y2="9"/></svg>`,
		target: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="6"/><circle cx="12" cy="12" r="2"/></svg>`,
		list: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><line x1="8" y1="6" x2="21" y2="6"/><line x1="8" y1="12" x2="21" y2="12"/><line x1="8" y1="18" x2="21" y2="18"/><line x1="3" y1="6" x2="3.01" y2="6"/><line x1="3" y1="12" x2="3.01" y2="12"/><line x1="3" y1="18" x2="3.01" y2="18"/></svg>`,
		link: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"/><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"/></svg>`,
		maximize: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M8 3H5a2 2 0 0 0-2 2v3m18 0V5a2 2 0 0 0-2-2h-3m0 18h3a2 2 0 0 0 2-2v-3M3 16v3a2 2 0 0 0 2 2h3"/></svg>`,
		externalLink: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>`,
	};
</script>

<div class="min-h-screen bg-white">
	<!-- Header -->
	<header class="flex items-center justify-between px-6 py-4 max-w-7xl mx-auto">
		<div class="flex items-center gap-2">
			<!-- Logo Icon -->
			<div class="text-primary-600">
				{@html icons.logo}
			</div>
			<span class="font-bold text-xl tracking-tight">Stacks</span>
		</div>
		<nav class="flex items-center gap-6 text-sm font-medium">
			<a href="#features" class="text-gray-600 hover:text-gray-900">Features</a>
			<a href="#pricing" class="text-gray-600 hover:text-gray-900">Pricing</a>
			<a href="https://app.betterstacks.com" class="bg-primary-600 text-white px-4 py-2 rounded-lg hover:bg-primary-700 transition-colors">Get Started</a>
		</nav>
	</header>

	<main>
		<!-- Hero Section -->
		<section class="max-w-4xl mx-auto px-6 pt-12 pb-20 text-center">
			<div class="inline-flex items-center gap-3 text-gray-500 text-sm mb-6 flex-wrap justify-center">
				<span class="flex items-center gap-1.5">
					<svg class="w-4 h-4" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/></svg>
					Chrome
				</span>
				<span class="text-gray-300">•</span>
				<span class="flex items-center gap-1.5">
					<svg class="w-4 h-4" viewBox="0 0 24 24" fill="currentColor"><path d="M17.6 9.48l1.84-3.18c.16-.31.25-.66.25-1.02 0-1.21-.99-2.2-2.2-2.2-.36 0-.71.09-1.02.25L13.29 5.1c-.23-.03-.46-.05-.69-.05-2.2 0-4.22.78-5.79 2.07L3.9 4.21c-.39-.39-1.02-.39-1.41 0-.39.39-.39 1.02 0 1.41l2.92 2.92C4.78 9.78 4 11.79 4 14c0 4.42 3.58 8 8 8s8-3.58 8-8c0-.46-.04-.92-.11-1.36l1.96-1.96c.39-.39.39-1.02 0-1.41-.39-.39-1.02-.39-1.41 0l-1.96 1.96c-.44-.8-.98-1.53-1.6-2.16zM12 20c-3.31 0-6-2.69-6-6s2.69-6 6-6 6 2.69 6 6-2.69 6-6 6z"/></svg>
					Android
				</span>
				<span class="text-gray-300">•</span>
				<span class="flex items-center gap-1.5">
					<svg class="w-4 h-4" viewBox="0 0 24 24" fill="currentColor"><path d="M17.05 20.28c-.98.95-2.05.8-3.08.35-1.09-.46-2.09-.48-3.24 0-1.44.62-2.2.44-3.06-.35C2.79 15.25 3.51 7.59 9.05 7.31c1.35.07 2.29.74 3.08.8 1.18-.24 2.31-.93 3.57-.84 1.51.12 2.65.72 3.4 1.8-3.12 1.87-2.38 5.98.48 7.13-.57 1.5-1.31 2.99-2.54 4.09l.01-.01zM12.03 7.25c-.15-2.23 1.66-4.07 3.74-4.25.29 2.58-2.34 4.5-3.74 4.25z"/></svg>
					iOS
				</span>
				<span class="text-gray-300">•</span>
				<span class="flex items-center gap-1.5">
					<svg class="w-4 h-4" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/></svg>
					Web
				</span>
			</div>
			
			<h1 class="text-5xl md:text-6xl font-bold tracking-tight text-gray-900 mb-6 leading-[1.1]">
				Your digital content, unified and understood
			</h1>
			
			<p class="text-xl text-gray-600 mb-10 max-w-2xl mx-auto">
				Stacks unifies scattered bookmarks, saves, and screenshots with intent-aware AI that remembers context and surfaces connections.
			</p>

			<div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-16">
				<a href="https://app.betterstacks.com" class="bg-primary-600 text-white px-8 py-3 rounded-xl font-semibold hover:bg-primary-700 transition-colors shadow-lg shadow-primary-600/20">
					Start Organizing Free
				</a>
				<a href="https://chrome.google.com/webstore" class="border border-gray-200 px-8 py-3 rounded-xl font-semibold hover:bg-gray-50 transition-colors flex items-center gap-2">
					<svg class="w-5 h-5" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/></svg>
					Add to Chrome
				</a>
			</div>

			<!-- Hero Image -->
			<div class="relative rounded-2xl border border-gray-200 shadow-2xl bg-white overflow-hidden mb-12">
				<img 
					src="/generated/image-knowledge-worker-at-modern-desk-with-mul-1765521059481-0.webp" 
					alt="Knowledge worker organizing digital content with Stacks"
					class="w-full h-auto"
				/>
			</div>

			<!-- Bottom Icons -->
			<div class="flex flex-wrap justify-center gap-8 md:gap-12 text-sm font-medium text-gray-700">
				<div class="flex items-center gap-2">
					{@html icons.search}
					<span>Natural search</span>
				</div>
				<div class="flex items-center gap-2">
					{@html icons.link}
					<span>Cross-platform</span>
				</div>
				<div class="flex items-center gap-2">
					{@html icons.sparkles}
					<span>AI-powered</span>
				</div>
				<div class="flex items-center gap-2">
					{@html icons.layout}
					<span>Team workspaces</span>
				</div>
			</div>
		</section>
		
		<!-- Features Grid -->
		<section id="features" class="max-w-6xl mx-auto px-6 py-20">
			<h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4 max-w-2xl leading-tight">
				Stop drowning in bookmarks. Start finding what matters.
			</h2>
			<p class="text-lg text-gray-600 mb-12 max-w-2xl">
				Trusted by 5,000+ creators, founders, and lifelong learners to organize 2.1M+ pieces of content.
			</p>

			<div class="grid grid-cols-1 md:grid-cols-3 gap-6">
				<!-- Card 1 -->
				<div class="bg-gray-50 p-8 rounded-2xl flex flex-col items-start h-64">
					<div class="mb-auto text-primary-600">
						{@html icons.link}
					</div>
					<div>
						<h3 class="font-bold text-lg mb-2 text-gray-900">Save from anywhere</h3>
						<p class="text-sm text-gray-600 leading-relaxed">Chrome extension, mobile apps, and web clipper work across all your devices</p>
					</div>
				</div>

				<!-- Card 2 -->
				<div class="bg-gray-50 p-8 rounded-2xl flex flex-col items-start h-64">
					<div class="mb-auto text-primary-600">
						{@html icons.sparkles}
					</div>
					<div>
						<h3 class="font-bold text-lg mb-2 text-gray-900">Intent-aware AI</h3>
						<p class="text-sm text-gray-600 leading-relaxed">Understands why you save content and surfaces relevant connections automatically</p>
					</div>
				</div>

				<!-- Card 3 -->
				<div class="bg-gray-50 p-8 rounded-2xl flex flex-col items-start h-64">
					<div class="mb-auto text-primary-600">
						{@html icons.layout}
					</div>
					<div>
						<h3 class="font-bold text-lg mb-2 text-gray-900">Smart organization</h3>
						<p class="text-sm text-gray-600 leading-relaxed">AI automatically extracts metadata, summarizes content, and organizes into workspaces</p>
					</div>
				</div>

				<!-- Card 4 -->
				<div class="bg-gray-50 p-8 rounded-2xl flex flex-col items-start h-64">
					<div class="mb-auto text-primary-600">
						{@html icons.search}
					</div>
					<div>
						<h3 class="font-bold text-lg mb-2 text-gray-900">Natural language search</h3>
						<p class="text-sm text-gray-600 leading-relaxed">Find content by meaning, not just keywords. Search understands context</p>
					</div>
				</div>

				<!-- Card 5 -->
				<div class="bg-gray-50 p-8 rounded-2xl flex flex-col items-start h-64">
					<div class="mb-auto text-primary-600">
						{@html icons.maximize}
					</div>
					<div>
						<h3 class="font-bold text-lg mb-2 text-gray-900">Team workspaces</h3>
						<p class="text-sm text-gray-600 leading-relaxed">Share collections with colleagues and collaborate on research</p>
					</div>
				</div>

				<!-- Card 6 -->
				<div class="bg-gray-50 p-8 rounded-2xl flex flex-col items-start h-64">
					<div class="mb-auto text-primary-600">
						{@html icons.target}
					</div>
					<div>
						<h3 class="font-bold text-lg mb-2 text-gray-900">Pattern recognition</h3>
						<p class="text-sm text-gray-600 leading-relaxed">AI spots patterns in your content you never noticed yourself</p>
					</div>
				</div>
			</div>
		</section>

		<!-- AI Features Section -->
		<section class="max-w-6xl mx-auto px-6 py-20">
			<div class="mb-16">
				<span class="inline-block bg-primary-100 text-primary-700 px-3 py-1 rounded-full text-xs font-semibold uppercase tracking-wide mb-6">
					Powered by 4.5M+ interaction data points
				</span>
				<h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6 tracking-tight">
					AI that understands your intent
				</h2>
				<p class="text-xl text-gray-600 max-w-2xl leading-relaxed">
					When you save content, you express an intention. Stacks AI understands that intent and helps you act on it.
				</p>
			</div>

			<div class="bg-primary-50/30 rounded-3xl p-8 md:p-12 mb-16">
				<div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
					<!-- Left Visual: Content Card -->
					<div class="relative bg-white rounded-2xl shadow-lg p-6 overflow-hidden min-h-[300px]">
						<div class="absolute top-0 left-0 w-full h-1 bg-gradient-to-r from-primary-500 to-primary-600"></div>
						<div class="flex items-center gap-2 mb-4 text-xs text-gray-400 border-b border-gray-100 pb-2">
							<div class="w-2 h-2 rounded-full bg-primary-500"></div>
							<span class="truncate">youtube.com/watch?v=dQw4w9WgXcQ</span>
						</div>
						<div class="space-y-4">
							<div>
								<h4 class="font-bold text-gray-900 mb-2">Building a Second Brain: Overview</h4>
								<div class="flex gap-2 mb-3">
									<span class="bg-primary-100 text-primary-700 px-2 py-0.5 rounded text-xs font-medium">Productivity</span>
									<span class="bg-primary-100 text-primary-700 px-2 py-0.5 rounded text-xs font-medium">Knowledge Management</span>
								</div>
								<p class="text-sm text-gray-600 leading-relaxed">
									Complete guide to organizing digital information for creative work. Covers capture, organize, distill, and express methodology.
								</p>
							</div>
							<div class="bg-primary-50/50 p-4 rounded-lg border border-primary-100">
								<div class="text-xs font-semibold text-primary-700 mb-2">AI DETECTED INTENT</div>
								<p class="text-xs text-gray-700">You're building a productivity system. This relates to 12 other items in your "Personal Knowledge" workspace.</p>
							</div>
							<div class="flex gap-2 text-xs text-gray-500">
								<span>Saved 2 days ago</span>
								<span>•</span>
								<span>From Chrome</span>
							</div>
						</div>
					</div>

					<!-- Right Visual: Connections -->
					<div class="bg-white rounded-2xl shadow-lg p-6 min-h-[300px] flex flex-col">
						<div class="mb-4">
							<h4 class="font-bold text-gray-900 mb-1">Related Content</h4>
							<p class="text-xs text-gray-500">AI found these connections</p>
						</div>
						<div class="flex-1 space-y-3">
							<div class="border border-gray-100 rounded-lg p-3 hover:border-primary-300 transition-colors cursor-pointer">
								<div class="flex items-start gap-2">
									<div class="w-8 h-8 rounded bg-gray-100 shrink-0"></div>
									<div class="flex-1 min-w-0">
										<h5 class="font-semibold text-sm text-gray-900 truncate">Notion Setup Guide</h5>
										<p class="text-xs text-gray-500 line-clamp-2">Your personal workspace setup from last month</p>
									</div>
								</div>
							</div>
							<div class="border border-gray-100 rounded-lg p-3 hover:border-primary-300 transition-colors cursor-pointer">
								<div class="flex items-start gap-2">
									<div class="w-8 h-8 rounded bg-gray-100 shrink-0"></div>
									<div class="flex-1 min-w-0">
										<h5 class="font-semibold text-sm text-gray-900 truncate">Zettelkasten Method</h5>
										<p class="text-xs text-gray-500 line-clamp-2">Note-taking system you bookmarked</p>
									</div>
								</div>
							</div>
							<div class="border border-gray-100 rounded-lg p-3 hover:border-primary-300 transition-colors cursor-pointer">
								<div class="flex items-start gap-2">
									<div class="w-8 h-8 rounded bg-gray-100 shrink-0"></div>
									<div class="flex-1 min-w-0">
										<h5 class="font-semibold text-sm text-gray-900 truncate">GTD Workflow</h5>
										<p class="text-xs text-gray-500 line-clamp-2">Getting Things Done methodology</p>
									</div>
								</div>
							</div>
						</div>
						<div class="mt-4 pt-4 border-t border-gray-100">
							<button class="text-xs text-primary-600 font-medium hover:text-primary-700">
								View all 12 connections →
							</button>
						</div>
					</div>
				</div>

				<!-- Bottom Visual: Search -->
				<div class="bg-white rounded-2xl shadow-lg p-6 md:p-8">
					<div class="relative mb-8">
						<input type="text" value="articles about building habits" class="w-full bg-gray-50 border-none rounded-xl py-4 pl-12 pr-4 text-gray-700 focus:ring-0" readonly />
						<div class="absolute left-4 top-1/2 -translate-y-1/2 text-gray-400">
							{@html icons.search}
						</div>
					</div>

					<div class="bg-primary-50/50 rounded-xl p-6 border border-primary-100">
						<div class="space-y-3">
							<div class="flex items-center gap-3">
								<div class="w-3 h-3 rounded-full bg-primary-500 animate-pulse"></div>
								<span class="text-sm text-gray-700">Searching your content...</span>
							</div>
							<div class="flex items-start gap-3">
								<div class="w-3 h-3 rounded-full bg-green-500 mt-1"></div>
								<div class="text-sm text-gray-700">
									<span class="font-medium">Found</span> 
									<span class="font-bold bg-white px-1 rounded border border-gray-200 mx-1">47 items</span> 
									about habit formation across 
									<span class="font-bold bg-white px-1 rounded border border-gray-200 mx-1">5 workspaces</span>
									<p class="text-xs text-gray-500 mt-1 max-w-md">Including related content about productivity, behavior change, and routine building.</p>
								</div>
							</div>
							<div class="flex items-center gap-3">
								<div class="w-3 h-3 rounded-full bg-green-500"></div>
								<span class="text-sm text-gray-700">Organized by <span class="bg-primary-500 text-white px-2 py-0.5 rounded text-xs font-bold">relevance</span></span>
							</div>
							<div class="flex items-center gap-3">
								<div class="w-3 h-3 rounded-full bg-green-500"></div>
								<span class="text-sm text-gray-700">Detected intent: <span class="text-primary-600 font-medium">Learning & Research</span></span>
							</div>
						</div>
					</div>
				</div>
			</div>

			<div class="grid grid-cols-1 md:grid-cols-2 gap-x-12 gap-y-4 max-w-4xl">
				<p class="text-xl text-gray-600 mb-6 md:col-span-2 leading-relaxed">
					Stacks AI processes millions of interactions to understand patterns in how you save and use content, surfacing connections you never knew existed.
				</p>
				
				<div class="space-y-4">
					<div class="flex items-center gap-3 text-primary-700 font-medium">
						{@html icons.sparkles}
						<span>Automatic metadata extraction</span>
					</div>
					<div class="flex items-center gap-3 text-primary-700 font-medium">
						{@html icons.target}
						<span>Intent signal detection</span>
					</div>
					<div class="flex items-center gap-3 text-primary-700 font-medium">
						{@html icons.layout}
						<span>Smart workspace organization</span>
					</div>
				</div>

				<div class="space-y-4">
					<div class="flex items-center gap-3 text-primary-700 font-medium">
						{@html icons.link}
						<span>Cross-platform content linking</span>
					</div>
					<div class="flex items-center gap-3 text-primary-700 font-medium">
						{@html icons.maximize}
						<span>Automatic summarization</span>
					</div>
					<div class="flex items-center gap-3 text-primary-700 font-medium">
						{@html icons.search}
						<span>Semantic search understanding</span>
					</div>
				</div>
			</div>
		</section>

		<!-- Workspaces Section -->
		<section class="max-w-6xl mx-auto px-6 py-20">
			<div class="mb-16">
				<span class="inline-block bg-primary-100 text-primary-700 px-3 py-1 rounded-full text-xs font-semibold uppercase tracking-wide mb-6">
					Collaboration
				</span>
				<h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6 tracking-tight">
					Organize and share with workspaces
				</h2>
				<p class="text-xl text-gray-600 max-w-2xl leading-relaxed">
					Create dedicated spaces for projects, share collections with your team, and collaborate on research.
				</p>
			</div>

			<div class="bg-primary-50/30 rounded-3xl p-8 md:p-12 mb-16">
				<div class="bg-white rounded-2xl shadow-sm p-6 md:p-8 max-w-3xl mx-auto">
					<!-- Workspace Header -->
					<div class="flex items-center justify-between mb-6">
						<div>
							<h3 class="text-xl font-bold text-gray-900">Product Research</h3>
							<p class="text-sm text-gray-500">Shared with 4 team members</p>
						</div>
						<button class="bg-primary-600 text-white px-4 py-2 rounded-lg text-sm font-medium hover:bg-primary-700">
							Share
						</button>
					</div>

					<!-- Folders -->
					<div class="space-y-3 mb-8">
						<div class="border border-gray-200 rounded-lg p-4 hover:border-primary-300 transition-colors cursor-pointer">
							<div class="flex items-center justify-between">
								<div class="flex items-center gap-3">
									{@html icons.layout}
									<div>
										<h4 class="font-semibold text-gray-900">Competitor Analysis</h4>
										<p class="text-xs text-gray-500">127 items • Updated 2h ago</p>
									</div>
								</div>
								<div class="flex -space-x-2">
									<div class="w-6 h-6 rounded-full bg-primary-200 border-2 border-white"></div>
									<div class="w-6 h-6 rounded-full bg-primary-300 border-2 border-white"></div>
								</div>
							</div>
						</div>

						<div class="border border-gray-200 rounded-lg p-4 hover:border-primary-300 transition-colors cursor-pointer">
							<div class="flex items-center justify-between">
								<div class="flex items-center gap-3">
									{@html icons.layout}
									<div>
										<h4 class="font-semibold text-gray-900">User Interviews</h4>
										<p class="text-xs text-gray-500">43 items • Updated yesterday</p>
									</div>
								</div>
								<div class="flex -space-x-2">
									<div class="w-6 h-6 rounded-full bg-primary-200 border-2 border-white"></div>
								</div>
							</div>
						</div>

						<div class="border border-gray-200 rounded-lg p-4 hover:border-primary-300 transition-colors cursor-pointer">
							<div class="flex items-center justify-between">
								<div class="flex items-center gap-3">
									{@html icons.layout}
									<div>
										<h4 class="font-semibold text-gray-900">Design Inspiration</h4>
										<p class="text-xs text-gray-500">89 items • Updated 3 days ago</p>
									</div>
								</div>
								<div class="flex -space-x-2">
									<div class="w-6 h-6 rounded-full bg-primary-200 border-2 border-white"></div>
									<div class="w-6 h-6 rounded-full bg-primary-300 border-2 border-white"></div>
									<div class="w-6 h-6 rounded-full bg-primary-400 border-2 border-white"></div>
								</div>
							</div>
						</div>
					</div>

					<!-- Recent Activity -->
					<div class="border-t border-gray-100 pt-6">
						<h4 class="text-sm font-semibold text-gray-900 mb-4">Recent Activity</h4>
						<div class="space-y-3 text-sm">
							<div class="flex items-start gap-3">
								<div class="w-6 h-6 rounded-full bg-primary-100 flex items-center justify-center shrink-0">
									<span class="text-xs font-bold text-primary-700">JD</span>
								</div>
								<div>
									<p class="text-gray-700"><span class="font-medium">John</span> added 5 items to Competitor Analysis</p>
									<p class="text-xs text-gray-500">2 hours ago</p>
								</div>
							</div>
							<div class="flex items-start gap-3">
								<div class="w-6 h-6 rounded-full bg-primary-100 flex items-center justify-center shrink-0">
									<span class="text-xs font-bold text-primary-700">SM</span>
								</div>
								<div>
									<p class="text-gray-700"><span class="font-medium">Sarah</span> shared this workspace with you</p>
									<p class="text-xs text-gray-500">Yesterday</p>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>

			<div class="flex flex-col md:flex-row gap-8 md:items-start justify-between">
				<div class="flex gap-6 text-sm font-medium text-gray-600">
					<div class="flex items-center gap-2">
						{@html icons.layout}
						<span>Unlimited workspaces</span>
					</div>
					<div class="flex items-center gap-2">
						{@html icons.maximize}
						<span>Team sharing</span>
					</div>
					<div class="flex items-center gap-2">
						{@html icons.link}
						<span>Public links</span>
					</div>
				</div>
				<p class="text-xl text-gray-600 max-w-lg leading-relaxed">
					Keep projects organized, share research with colleagues, and collaborate without losing context.
				</p>
			</div>
		</section>

		<!-- Pricing Section -->
		<section id="pricing" class="max-w-6xl mx-auto px-6 py-20">
			<div class="text-center mb-16">
				<h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6 tracking-tight">
					Simple, transparent pricing
				</h2>
				<p class="text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
					Start free, upgrade when you need more. 30-day money-back guarantee, no questions asked.
				</p>
			</div>

			<div class="grid grid-cols-1 md:grid-cols-3 gap-6">
				<!-- Free Plan -->
				<div class="border border-gray-200 rounded-2xl p-8 hover:border-primary-300 transition-colors">
					<h3 class="text-xl font-bold text-gray-900 mb-2">Free</h3>
					<div class="mb-6">
						<span class="text-4xl font-bold text-gray-900">$0</span>
						<span class="text-gray-500">/month</span>
					</div>
					<ul class="space-y-3 mb-8 text-sm">
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Up to 1,000 items</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Basic AI features</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Chrome extension</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Mobile apps</span>
						</li>
					</ul>
					<button class="w-full py-3 border border-gray-200 rounded-lg font-semibold hover:bg-gray-50 transition-colors">
						Get Started
					</button>
				</div>

				<!-- Pro Plan -->
				<div class="border-2 border-primary-600 rounded-2xl p-8 relative">
					<div class="absolute -top-4 left-1/2 -translate-x-1/2 bg-primary-600 text-white px-4 py-1 rounded-full text-xs font-semibold">
						MOST POPULAR
					</div>
					<h3 class="text-xl font-bold text-gray-900 mb-2">Be Productive</h3>
					<div class="mb-6">
						<span class="text-4xl font-bold text-gray-900">$9</span>
						<span class="text-gray-500">/month</span>
						<div class="text-xs text-gray-500 mt-1">or $89/year (save 30%)</div>
					</div>
					<ul class="space-y-3 mb-8 text-sm">
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Unlimited items</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Advanced AI features</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Priority support</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">All platforms</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Workspace sharing</span>
						</li>
					</ul>
					<button class="w-full py-3 bg-primary-600 text-white rounded-lg font-semibold hover:bg-primary-700 transition-colors">
						Start Free Trial
					</button>
				</div>

				<!-- Team Plan -->
				<div class="border border-gray-200 rounded-2xl p-8 hover:border-primary-300 transition-colors">
					<h3 class="text-xl font-bold text-gray-900 mb-2">Be Collaborative</h3>
					<div class="mb-6">
						<span class="text-4xl font-bold text-gray-900">$29</span>
						<span class="text-gray-500">/month</span>
						<div class="text-xs text-gray-500 mt-1">or $199/year</div>
					</div>
					<ul class="space-y-3 mb-8 text-sm">
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Everything in Pro</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Team workspaces</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Priority chat support</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Admin controls</span>
						</li>
						<li class="flex items-start gap-2">
							{@html icons.check}
							<span class="text-gray-600">Advanced analytics</span>
						</li>
					</ul>
					<button class="w-full py-3 border border-gray-200 rounded-lg font-semibold hover:bg-gray-50 transition-colors">
						Start Free Trial
					</button>
				</div>
			</div>

			<div class="text-center mt-12">
				<p class="text-sm text-gray-600 mb-4">Need more? <a href="mailto:enterprise@betterstacks.com" class="text-primary-600 font-semibold hover:text-primary-700">Contact us for Enterprise pricing</a></p>
				<div class="flex items-center justify-center gap-6 text-xs text-gray-500">
					<span class="flex items-center gap-2">
						{@html icons.check}
						30-day money-back guarantee
					</span>
					<span class="flex items-center gap-2">
						{@html icons.check}
						Cancel anytime
					</span>
					<span class="flex items-center gap-2">
						{@html icons.check}
						No credit card required
					</span>
				</div>
			</div>
		</section>

		<!-- Use Cases & Testimonials Section -->
		<section class="max-w-7xl mx-auto px-6 py-20">
			<div class="mb-16">
				<span class="inline-block bg-gray-100 text-gray-700 px-3 py-1 rounded-full text-xs font-semibold uppercase tracking-wide mb-6">
					Trusted by knowledge workers
				</span>
				<h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6 tracking-tight">
					Built for how you actually work
				</h2>
				<p class="text-xl text-gray-600 max-w-2xl leading-relaxed">
					From researchers to creators to founders, Stacks helps organize the content that matters.
				</p>
			</div>

			<!-- Testimonials -->
			<div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-16">
				<div class="bg-gray-50 p-6 rounded-xl">
					<div class="flex items-center gap-3 mb-4">
						<div class="w-10 h-10 rounded-full bg-primary-200"></div>
						<div>
							<div class="font-semibold text-gray-900">Guta Raspanti</div>
							<div class="text-xs text-gray-500">Visionary</div>
						</div>
					</div>
					<p class="text-sm text-gray-700 mb-3">"My bookmarks were scattered across platforms with no connection. Stacks understood what I was trying to accomplish."</p>
					<div class="text-xs font-semibold text-primary-600">Saved 2+ hours daily</div>
				</div>

				<div class="bg-gray-50 p-6 rounded-xl">
					<div class="flex items-center gap-3 mb-4">
						<div class="w-10 h-10 rounded-full bg-primary-200"></div>
						<div>
							<div class="font-semibold text-gray-900">Chase DiMarco</div>
							<div class="text-xs text-gray-500">Researcher</div>
						</div>
					</div>
					<p class="text-sm text-gray-700 mb-3">"I can create workspaces, folders within each, and share them with my team easily. Game changer for collaboration."</p>
					<div class="text-xs font-semibold text-primary-600">Shared 50+ workspaces</div>
				</div>

				<div class="bg-gray-50 p-6 rounded-xl">
					<div class="flex items-center gap-3 mb-4">
						<div class="w-10 h-10 rounded-full bg-primary-200"></div>
						<div>
							<div class="font-semibold text-gray-900">Mohit Baid</div>
							<div class="text-xs text-gray-500">Innovator</div>
						</div>
					</div>
					<p class="text-sm text-gray-700 mb-3">"The product recognizes patterns in my content I never noticed. Like having an assistant that understands why I save things."</p>
					<div class="text-xs font-semibold text-primary-600">Found 200+ connections</div>
				</div>
			</div>

			<!-- Use Cases -->
			<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
				<!-- Card 1 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Research Organization</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Collect articles, papers, and resources for projects. AI finds connections across sources.</p>
				</div>
				<!-- Card 2 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Content Curation</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Save inspiration from social media, blogs, and videos. Build collections by theme.</p>
				</div>
				<!-- Card 3 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Team Knowledge Base</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Share resources with colleagues. Build shared understanding across your team.</p>
				</div>
				<!-- Card 4 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Learning Paths</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Organize tutorials, courses, and guides. Track your learning journey over time.</p>
				</div>

				<!-- Card 5 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Product Research</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Collect competitor analysis, user feedback, and market insights in one place.</p>
				</div>
				<!-- Card 6 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Design Inspiration</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Save examples, screenshots, and references. Find them when you need them.</p>
				</div>
				<!-- Card 7 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Reading Lists</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Save articles to read later. AI summarizes and extracts key points automatically.</p>
				</div>
				<!-- Card 8 -->
				<div class="bg-gray-100 p-6 rounded-xl min-h-[180px] flex flex-col">
					<h3 class="font-bold text-gray-900 mb-2">Project Planning</h3>
					<p class="text-xs text-gray-600 mt-auto leading-relaxed">Gather requirements, specs, and references. Keep everything accessible to your team.</p>
				</div>
			</div>
		</section>

		<!-- Final CTA Section -->
		<section class="max-w-4xl mx-auto px-6 py-20">
			<div class="bg-gradient-to-br from-primary-600 to-primary-700 rounded-3xl p-12 text-center text-white">
				<h2 class="text-3xl md:text-4xl font-bold mb-4">
					Stop losing track of what matters
				</h2>
				<p class="text-lg text-primary-50 mb-8 max-w-2xl mx-auto">
					Join 5,000+ knowledge workers who've organized over 2.1M pieces of content with Stacks.
				</p>
				<div class="flex flex-col sm:flex-row items-center justify-center gap-4">
					<a href="https://app.betterstacks.com" class="bg-white text-primary-600 px-8 py-3 rounded-xl font-semibold hover:bg-primary-50 transition-colors shadow-lg">
						Start Organizing Free
					</a>
					<a href="https://chrome.google.com/webstore" class="border-2 border-white text-white px-8 py-3 rounded-xl font-semibold hover:bg-white/10 transition-colors">
						Add to Chrome
					</a>
				</div>
				<p class="text-sm text-primary-100 mt-6">
					No credit card required • Free forever plan available
				</p>
			</div>
		</section>

		<!-- Footer -->
		<footer class="max-w-7xl mx-auto px-6 py-12 border-t border-gray-100">
			<div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-12">
				<div>
					<div class="flex items-center gap-2 mb-4">
						<div class="text-primary-600">
							{@html icons.logo}
						</div>
						<span class="font-bold text-lg">Stacks</span>
					</div>
					<p class="text-xs text-gray-600 leading-relaxed">
						Unifying scattered digital content with intent-aware AI.
					</p>
				</div>
				
				<div>
					<h4 class="font-bold text-sm text-gray-900 mb-4">Product</h4>
					<div class="space-y-2 text-xs text-gray-600">
						<a href="#features" class="block hover:text-gray-900">Features</a>
						<a href="#pricing" class="block hover:text-gray-900">Pricing</a>
						<a href="https://chrome.google.com/webstore" class="block hover:text-gray-900">Chrome Extension</a>
						<a href="https://apps.apple.com" class="block hover:text-gray-900">Mobile Apps</a>
					</div>
				</div>

				<div>
					<h4 class="font-bold text-sm text-gray-900 mb-4">Company</h4>
					<div class="space-y-2 text-xs text-gray-600">
						<a href="#" class="block hover:text-gray-900">About</a>
						<a href="#" class="block hover:text-gray-900">Blog</a>
						<a href="mailto:enterprise@betterstacks.com" class="block hover:text-gray-900">Enterprise</a>
						<a href="mailto:help@betterstacks.com" class="block hover:text-gray-900">Support</a>
					</div>
				</div>

				<div>
					<h4 class="font-bold text-sm text-gray-900 mb-4">Legal</h4>
					<div class="space-y-2 text-xs text-gray-600">
						<a href="#" class="block hover:text-gray-900">Privacy Policy</a>
						<a href="#" class="block hover:text-gray-900">Terms of Service</a>
						<a href="#" class="block hover:text-gray-900">Security</a>
					</div>
				</div>
			</div>

			<div class="flex flex-col md:flex-row justify-between items-center pt-8 border-t border-gray-100 text-xs text-gray-500">
				<div class="mb-4 md:mb-0">
					<p>© 2025 Stacks. All rights reserved.</p>
				</div>
				<div class="flex items-center gap-4">
					<span class="bg-green-100 text-green-700 px-3 py-1 rounded-full font-medium flex items-center gap-1">
						<span class="w-2 h-2 rounded-full bg-green-500"></span>
						All Systems Operational
					</span>
				</div>
			</div>
		</footer>

	</main>
</div>

