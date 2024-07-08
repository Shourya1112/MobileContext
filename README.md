##MobileContext

just a simple react file using context api to know in any component wheather the screen is desktop or on mobile.

steps:
1. paste mobileContext.ts in utils folder
2. import dependencies
3. wrap app.js files or routes in <MobileProvider>.
4. use "const { isMobile } = useMobile();" in any file. Don't forget to import { useMobile }


PS: will add further device and other device info later...
