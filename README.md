# Ansible Role: Create Lets Encrypt certificate with Cloudflare DNS

[![Build Status](https://travis-ci.org/dsgnr/ansible-role-letsencrypt-wildcard-certificate.svg?branch=master)](https://travis-ci.org/dsgnr/ansible-role-letsencrypt-wildcard-certificate)

Utilises Lets Encrypt and Cloudflare DNS to deploy wildcard (or standard) SSL certificates.

## Requirements

None.

## Role Variables

certificate_tld: "put the root of your domain here"

cloudflare_email: "put your Cloudflare email here"

cloudflare_api_key: "put your Cloudflare global API key here"

cloudflare_domain: "{{ certificate_tld }}"

## Dependencies

None.

## Example Playbook

    - hosts: all
      become: true
      
      roles:
        - deploy-letsencrypt-wildcard-certificate

## License

GNUv3

