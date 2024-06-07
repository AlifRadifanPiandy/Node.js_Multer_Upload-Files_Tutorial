# Node.js File Upload Tutorial with Multer

This project is a simple Node.js application that demonstrates how to upload multiple files using Multer.

## Project Structure

The project is organized as follows:

- **.gitignore:** Specifies the files and directories that Git should ignore.
- **package.json:** Contains the metadata of the project and its dependencies.
- **README.md:** This file.
- **src/:** The source code of the application.
  - **controllers/:** Contains the logic for handling requests.
    - **home.js:** Handles requests to the home page.
    - **upload.js:** Handles file upload requests.
  - **middleware/:** Contains middleware functions.
    - **upload.js:** Contains the middleware for handling file uploads.
  - **routes/:** Contains the application's routes.
    - **web.js:** Defines the application's routes.
  - **server.js:** The entry point of the application.
  - **views/:** Contains the HTML files for the application's views.
    - **index.html:** The home page of the application.
  - **upload/:** The directory where uploaded files are stored.

## How It Works

When a user visits the home page, they are presented with a form that allows them to select multiple files for upload. When the form is submitted, the files are uploaded to the server and stored in the `upload/` directory.

The file upload is handled by the `upload` and `multipleUpload` functions in the `upload.js` controller. The `uploadFiles` and `uploadFilesMiddleware` middleware functions are used to process the uploaded files.

The application's routes are defined in the `web.js` file and are initialized in the `initRoutes` function in the `server.js` file.

## Running the Application

To run the application, use the start script defined in the `package.json` file:

```bash
npm start
```

The application will start and listen on port 3000.

## Dependencies

This application uses the following dependencies:

- **express:** A fast, unopinionated, and flexible Node.js web application framework.
- **multer:** A middleware for handling `multipart/form-data`, which is primarily used for uploading files.

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
