# ProjetoFormsCadastro
CRIE UM PROJETO DE FORMA QUE CAPTURE NOME, DATA DE NASCIMENTO, CPF E TELEFONE E AO CLICAR EM UM BOTÃO, EXIBA EM LABEL´S DIFERENTES OS DADOS  INFORMADOS NAS TEXTBOX´S.
NÃO ESQUEÇA DE CRIAR O BOTÃO DE LIMPAR CAMPOS.

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace ProjetoFormsCadastro
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

  private void btnExibir_Click(object sender, EventArgs e)
        {
            lblNome.Text = "Nome: " + txtNome.Text;
            lblDataNasc.Text = "Data de Nascimento: " + txtDataNasc.Text;
            lblCPF.Text = "CPF: " + txtCPF.Text;
            lblTelefone.Text = "Telefone: " + txtTelefone.Text;
        }

  private void btnLimpar_Click(object sender, EventArgs e)
        {
            txtNome.Clear();
            txtDataNasc.Clear();
            txtCPF.Clear();
            txtTelefone.Clear();

  lblNome.Text = "Nome: ";
            lblDataNasc.Text = "Data de Nascimento: ";
            lblCPF.Text = "CPF: ";
            lblTelefone.Text = "Telefone: ";
        }
    }
}
