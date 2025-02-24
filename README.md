docker run -it -v C:\Users\ASUS\Downloads\my_model\my_model:/models -p 8501:8501 --entrypoint /bin/bash tensorflow/serving
tensorflow_model_server --rest_api_port=8501 --model_name=my_model --model_base_path=/models/my_model/

# Hasil yang ditampilkan dilocal #

{
  "model_version_status": [
    {
      "version": "1",
      "state": "AVAILABLE",
      "status": {
        "error_code": "OK",
        "error_message": ""
      }
    }
  ]
}



