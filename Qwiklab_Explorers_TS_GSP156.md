# Terraform Fundamentals || [GSP156](https://www.cloudskillsboost.google/games/5396/labs/35019) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

### Run the following Commands in CloudShell

```
export ZONE=
```
```
gcloud auth list 

cat > instance.tf <<EOF_END
resource "google_compute_instance" "terraform" {
  project      = "$DEVSHELL_PROJECT_ID"
  name         = "terraform"
  machine_type = "e2-medium"
  zone         = "$ZONE"

  boot_disk {
    initialize_params {
      image = "debian-cloud/debian-11"
    }
  }

  network_interface {
    network = "default"
    access_config {
    }
  }
}
EOF_END

terraform init
terraform plan
terraform apply --auto-approve
```

# Congratulations ..!!🎉  You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN)
