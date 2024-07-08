# MobileContext

A simple React utility using the Context API to determine if the screen is on a desktop or mobile device. 

## Steps

1. **Add the `mobileContext.ts` file:**
   - Place the `mobileContext.ts` file in your `utils` folder.

2. **Import dependencies:**
   - Ensure you import the necessary dependencies in your project.

3. **Wrap your application:**
   - Wrap your `App.js` or your main routes file with the `MobileProvider` context provider.
     ```jsx
     import { MobileProvider } from './utils/mobileContext';

     function App() {
       return (
         <MobileProvider>
           {/* Your routes or main component */}
         </MobileProvider>
       );
     }
     ```

4. **Use the context in your components:**
   - To use the mobile context in any component, use the following code:
     ```jsx
     import { useMobile } from './utils/mobileContext';

     const YourComponent = () => {
       const { isMobile } = useMobile();

       return (
         <div>
           {isMobile ? 'Mobile view' : 'Desktop view'}
         </div>
       );
     };
     ```

## Notes
- Additional device information and support for other devices will be added in the future...
