<template>
	<main class="grid justify-items-center">
		<div class="flex justify-center md:w-8/12 dark:bg-slate-300  rounded-lg shadow-lg p-8">
			<img
				class="w-32 h-32 rounded-full object-cover mr-4"
				src="@/assets/profile_pic.jpg"
				alt="profile_pic"
			/>
			<div>
				<h1 class="text-xl font-bold mb-2">David Bong Xia Shing</h1>
				<p class="text-gray-600">Future Software Developer</p>
				<p class="mt-2 text-gray-600">
					I am currently in my <b>final semester</b> of my
					<b>
						Bachelor of Computer Science (Software Engineering) student with
						Honours
					</b>
					from <i>Universiti Malaysia Sarawak</i>. I am looking for a
					<b>fulltime software developer</b> role to begin the next chapter of
					my life. 
				</p>
				<p class="text-gray-600 mt-3 font-semibold">Expected Graduation: July 2023</p>
				<p class="text-gray-600">
					<h4 class="font-bold mt-3">My Tech Stack</h4>
					<ul class="list-disc">
						<li class="ms-6"><span class="font-semibold text-gray-600">Languages:</span> JavaScript, PHP, Solidity, C/C++</li> 
						<li class="ms-6"><span class="font-semibold text-gray-600">Frontend:</span> Vue.js, HTML, CSS, Bootstrap, Tailwind CSS</li>
						<li class="ms-6"><span class="font-semibold text-gray-600">Backend:</span> Laravel, Node.js, Express.js, MongoDB, MySQL</li>
						<li class="ms-6"><span class="font-semibold text-gray-600">Others:</span> Git, GitHub, Heroku, Netlify</li>
					</ul>
				</p>
				<p class="mt-2 text-gray-600">
					<b>Contact:</b> davidbong05@gmail.com
				</p>
				<div class="mt-4 flex">
					<button
						onclick="window.location.href='https://github.com/davidbong-05'"
						class="flex me-2 rounded-md dark:bg-slate-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
					>
						<svg
							viewBox="0 0 24 24"
							xmlns="http://www.w3.org/2000/svg"
							fill="currentColor"
							class="h-5 w-5 me-2"
						>
							<path
								d="M12 .298C5.37.298 0 5.675 0 12.306c0 5.406 3.438 9.98 8.205 11.583.6.112.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61-.546-1.39-1.332-1.76-1.332-1.76-1.088-.743.083-.727.083-.727 1.203.085 1.838 1.237 1.838 1.237 1.07 1.836 2.81 1.304 3.495.997.108-.776.418-1.305.76-1.605-2.665-.306-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.307-.54-1.53.105-3.182 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.4 3-.405 1.02.005 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.652.24 2.875.12 3.182.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.62-5.475 5.92.42.36.81 1.096.81 2.22 0 1.607-.015 2.897-.015 3.287 0 .315.21.69.825.57C20.565 22.28 24 17.707 24 12.305c0-6.63-5.373-12.008-12-12.008z"
							/>
						</svg>
						GitHub
					</button>
					<button
						onclick="window.location.href='https://www.linkedin.com/in/davidbong05/'"
						class="flex rounded-md dark:bg-blue-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
					>
						<svg
							viewBox="0 0 16 16"
							xmlns="http://www.w3.org/2000/svg"
							fill="currentColor"
							class="h-5 w-5 mt-0.5 me-2"
						>
							<path
								d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"
							/>
						</svg>
						LinkedIn
					</button>
				</div>
			</div>
		</div>

		<div class="mt-10 md:w-full sm:mx-auto sm:w-full sm:max-w-sm">
			<p class="mb-4 text-slate-900 dark:text-white">
				Get my resume and CV from the faucet below: 
			</p>
			<form class="space-y-6" action="#">
				<div class="md:flex md:justify-center w-full">
					<label
						for="email"
						class="text-sm mt-2 me-2 font-medium md:leading-9 text-slate-900 dark:text-white sm:text-sm sm:leading-6"
						>Email</label
					>
					<input
						type="email"
						v-model="email"
						required
						class="w-full mt-2 me-2 rounded-md border-0 px-2 py-1.5 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
						placeholder="example@email.com"
					/>
					<button
						type="submit"
						@click.prevent="send"
						class="mt-2 rounded-md dark:bg-slate-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
					>
						Send
					</button>
				</div>
				<div class="mt-2 text-slate-900 dark:text-white text-xs">* It will be send to your inbox instantly</div>
			</form>
		</div>
		<div
			class="my-3 inline-flex w-full items-center rounded-lg bg-success-800 px-6 py-5 text-base text-neutral-50 dark:bg-neutral-900"
			role="alert"
			v-if="success"
		>
			<span class="mr-2">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="currentColor"
					class="h-5 w-5"
				>
					<path
						fill-rule="evenodd"
						d="M2.25 12c0-5.385 4.365-9.75 9.75-9.75s9.75 4.365 9.75 9.75-4.365 9.75-9.75 9.75S2.25 17.385 2.25 12zm13.36-1.814a.75.75 0 10-1.22-.872l-3.236 4.53L9.53 12.22a.75.75 0 00-1.06 1.06l2.25 2.25a.75.75 0 001.14-.094l3.75-5.25z"
						clip-rule="evenodd"
					/>
				</svg>
			</span>
			Thank you! Please check your email inbox.
		</div>
		<div
			class="my-3 inline-flex w-full items-center rounded-lg bg-danger-100 px-6 py-5 text-base text-neutral-50 dark:bg-neutral-900"
			role="alert"
			v-if="error"
		>
			<span class="mr-2">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="currentColor"
					class="h-5 w-5"
				>
					<path
						fill-rule="evenodd"
						d="M9.401 3.003c1.155-2 4.043-2 5.197 0l7.355 12.748c1.154 2-.29 4.5-2.599 4.5H4.645c-2.309 0-3.752-2.5-2.598-4.5L9.4 3.003zM12 8.25a.75.75 0 01.75.75v3.75a.75.75 0 01-1.5 0V9a.75.75 0 01.75-.75zm0 8.25a.75.75 0 100-1.5.75.75 0 000 1.5z"
						clip-rule="evenodd"
					/>
				</svg>
			</span>
			Sorry! It seems like theres an error. Please try again later.
		</div>
	</main>
</template>
<script>
	import { ref } from "vue";
	import emailjs from "@emailjs/browser";
	export default {
		setup() {
			const email = ref("");
			const success = ref(false);
			const error = ref(false);

			const send = async () => {
				const data = {
					to_email: email.value,
					message: "Check this out!",
				};
				try {
					const res = await emailjs.send(
						import.meta.env.VITE_EMAIL_SERVICE_ID,
						import.meta.env.VITE_EMAIL_TEMPLATE_ID,
						data,
						import.meta.env.VITE_EMAIL_PUBLIC_KEY
					);
					if (res.status === 200) success.value = true;
					else error.value = true;
				} catch (error) {
					console.log({ error });
				}
				email.value = "";
			};

			return {
				email,
				success,
				error,
				send,
			};
		},
	};
</script>
