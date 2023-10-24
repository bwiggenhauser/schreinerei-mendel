<script>
	const projects = [
		{
			name: "Projekt 1",
			description:
				"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl."
		},
		{
			name: "Projekt 2",
			description:
				"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl."
		},
		{
			name: "Projekt 3",
			description:
				"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni sl. Nulla euismod, nisl vitae aliquam ultricies, nunc nisl aliquet nunc, vitae aliquam nisl nisl vitae ni."
		}
	];
</script>

<div class="flex flex-col justify-start items-center my-8 gap-8">
	{#each projects as project}
		<div class="flex flex-col items-center w-full px-8 gap-4">
			<div class="flex flex-col items-center md:items-start gap-4 md:flex-row md:justify-between">
				<img src="/placeholder.jpg" alt="placeholder" class="md:w-1/2 h-auto" />
				<div class="hidden md:block w-4" />
				<div class="md:w-1/2">
					<h2 class="font-bold text-xl text-center md:text-left leading-none mb-3">
						{project.name}
					</h2>
					<p class="text-sm text-center md:text-left">{project.description}</p>
				</div>
			</div>
		</div>
	{/each}
</div>
